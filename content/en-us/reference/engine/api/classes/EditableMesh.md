---
title: EditableMesh
type: class
superclass: Object
tags: [NotCreatable]
---

# EditableMesh

Object which allows for the runtime creation and manipulation of meshes.

**Inherits from:** `Class.Object`

**Tags:** [NotCreatable]

## Description

`EditableMesh` changes the applied visual mesh when linked to a
`Class.MeshPart`, allowing for querying and modification of the mesh both in
Studio and in-game.

#### Enabling for published games

For security purposes, using `EditableMesh` fails by default for published
games. To enable usage of `EditableMesh`, you must be 13+ age verified and ID
verified. After you are verified, open Studio's
[Experience Settings](../../../studio/experience-settings.md), select
**Security**, and enable the **Allow&nbsp;Mesh&nbsp;&&nbsp;Image&nbsp;APIs**
toggle. Remember to review the
[Terms of Use](https://en.help.roblox.com/hc/en-us/articles/115004647846-Roblox-Terms-of-Use#creators-restrictions-on-use)
before enabling the toggle.

#### Permissions

To prevent misuse, `Class.AssetService:CreateEditableMeshAsync()` only allows
you to load and edit mesh assets if any of the following is true:

- Owned by or explicitly shared with the game owner.
- Owned by or explicitly shared with the logged in Studio user.
- Owned by or explicitly shared with the logged in player if the
  `EditableMesh` is on the client side.
- Owned by a group where the game owner, Studio user, or player has a role
  with permission to edit the group's assets. See
  [Roles and permissions](../../../projects/groups.md#roles-and-permissions)
  for more information.

See [Grant permissions](../../../projects/assets/privacy.md#grant-permissions)
to learn how to share assets with users or groups.

The APIs throw an error if they are used to load an asset that does not meet
the criteria above.

#### Memory limits

Editable assets are currently expensive for memory usage. To minimize its
impact on client performance, `EditableMesh` has strict client-side memory
budgets, although the server, Studio, and plugins operate with unlimited
memory. Using `Class.EditableMesh.FixedSize|FixedSize` may help you stay
within the memory budget and, in some scenarios, linking one `EditableMesh` to
multiple `Class.MeshPart|MeshParts` (multi-referencing) can help with memory
optimization.

#### Creation and display

An `EditableMesh` can be created from an existing `Datatype.Content` of a
`Class.MeshPart` or a mesh ID using
`Class.AssetService:CreateEditableMeshAsync()`, or a blank `EditableMesh` can
be created with `Class.AssetService:CreateEditableMesh()`. It can then be
displayed, modified, and its collision model updated. Not all of the steps are
necessary; for example, you might want to create an `EditableMesh` just to
raycast without ever displaying it.

```lua
local AssetService = game:GetService("AssetService")

-- Create empty EditableMesh
local editableMesh = AssetService:CreateEditableMesh()

-- Create EditableMesh from asset ID
local editableMeshFromAsset = nil
local success, errorMessage = pcall(function()
	editableMeshFromAsset = AssetService:CreateEditableMeshAsync(Content.fromAssetId(ASSET_ID))
end)

-- Create EditableMesh from another EditableMesh
local editableMeshFromAnother = nil
local success, errorMessage = pcall(function()
	editableMeshFromAnother = AssetService:CreateEditableMeshAsync(Content.fromObject(OTHER_EDITABLE_MESH))
end)

-- Create EditableMesh from MeshPart
local editableMeshFromMeshPart = nil
local success, errorMessage = pcall(function()
	editableMeshFromMeshPart = AssetService:CreateEditableMeshAsync(MESH_PART.MeshContent)
end)
```

An `EditableMesh` is displayed when it's linked to a new `Class.MeshPart`,
through `Class.AssetService:CreateMeshPartAsync()`. You can create more
`Class.MeshPart` instances that reference the same `EditableMesh`
`Datatype.Content`, or link to an existing `Class.MeshPart` through
`Class.MeshPart:ApplyMesh()`.

```lua
local AssetService = game:GetService("AssetService")
local Workspace = game:GetService("Workspace")

-- Create EditableMesh from asset ID
local editableMeshFromAsset = nil
local success, errorMessage = pcall(function()
	editableMeshFromAsset = AssetService:CreateEditableMeshAsync(Content.fromAssetId(ASSET_ID))
end)

-- Create new MeshPart linked to the EditableMesh
local newMeshPart = nil
local success, errorMessage = pcall(function()
	newMeshPart = AssetService:CreateMeshPartAsync(Content.fromObject(editableMeshFromAsset))
end)

-- Alternatively, link the new MeshPart created above to an existing MeshPart
local existingMeshPart = Workspace:FindFirstChild("EXISTING_MESH_PART")
existingMeshPart:ApplyMesh(newMeshPart)
```

To recalculate collision and fluid geometry after editing, you can again call
`Class.AssetService:CreateMeshPartAsync()` and `Class.MeshPart:ApplyMesh()` to
update an existing `Class.MeshPart`. It's generally recommended to do this at
the end of a conceptual edit, not after individual calls to methods that
manipulate geometry. Visual changes to the mesh will always be immediately
reflected by the engine, without the need to call
`Class.AssetService:CreateMeshPartAsync()`.

#### Fixed-size meshes

When creating an `EditableMesh` from an existing mesh asset (via
`Class.AssetService:CreateEditableMeshAsync()`), the resulting editable mesh
is fixed-size by default. Fixed-size meshes are more efficient in terms of
memory but you cannot change the number of vertices, faces, or attributes.
Only the values of vertex attributes and positions can be edited.

```lua
local AssetService = game:GetService("AssetService")

-- Create EditableMesh without fixed-size default
local editableMeshFromAsset = nil
local success, errorMessage = pcall(function()
	editableMeshFromAsset = AssetService:CreateEditableMeshAsync(Content.fromAssetId(ASSET_ID), {FixedSize = false})
end)
```

#### Stable vertex/face IDs

Many `EditableMesh` methods take **vertex**, **normal**, **UV**, **color** and
**face** IDs. These are represented as integers in Luau but they require some
special handling. The main difference is that IDs are stable and they remain
the same even if other parts of the mesh change. For example, if an
`EditableMesh` has five vertices `{1, 2, 3, 4, 5}` and you remove vertex `4`,
the new vertices will be `{1, 2, 3, 5}`.

Note that the IDs are not guaranteed to be in order and there may be holes in
the numbering, so when iterating through vertices or faces, you should iterate
through the table returned by `Class.EditableMesh:GetVertices()|GetVertices()`
or `Class.EditableMesh:GetFaces()|GetFaces()`.

#### Split vertex attributes

A **vertex** is a corner of a face, and topologically connects faces together.
Vertices can have several attributes: position, normal, UV coordinate, color,
and transparency.

Sometimes it's useful for all faces that touch a vertex to use the same
attribute values, but sometimes you'll want different faces to use different
attribute values on the same vertex. For example, on a smooth sphere, each
vertex will only have a single normal. In contrast, at the corner of a cube,
the vertex will have 3 different normals (one for each adjacent face). You can
also have seams in the UV coordinates or sharp changes in the vertex colors.

When creating faces with `Class.EditableMesh:AddTriangle()|AddTriangle()`,
each corner of the new face is automatically assigned a normal, UV, and color
attribute. If a vertex already belongs to an existing face, the new face
**reuses** that vertex's existing attributes (producing smooth shading and
continuous UVs). If the vertex is new, fresh attribute IDs are created with
default values (auto-computed normal, UV of `(0, 0)`, white color). To create
a seam, you should create new attributes and set them on the face. For
example, this code will create a sharp cube:

```lua
local AssetService = game:GetService("AssetService")

-- Given 4 vertex IDs, adds a new normal and 2 triangles, making a sharp quad
local function addSharpQuad(editableMesh, vid0, vid1, vid2, vid3)
	local nid = editableMesh:AddNormal()  -- This creates a normal ID which is automatically computed

	local fid1 = editableMesh:AddTriangle(vid0, vid1, vid2)
	editableMesh:SetFaceNormals(fid1, {nid, nid, nid})

	local fid2 = editableMesh:AddTriangle(vid0, vid2, vid3)
	editableMesh:SetFaceNormals(fid2, {nid, nid, nid})
end

-- Makes a cube with creased edges between the 6 sides
local function makeSharpCube()
	local editableMesh = AssetService:CreateEditableMesh()

	local v1 = editableMesh:AddVertex(Vector3.new(0, 0, 0))
	local v2 = editableMesh:AddVertex(Vector3.new(1, 0, 0))
	local v3 = editableMesh:AddVertex(Vector3.new(0, 1, 0))
	local v4 = editableMesh:AddVertex(Vector3.new(1, 1, 0))
	local v5 = editableMesh:AddVertex(Vector3.new(0, 0, 1))
	local v6 = editableMesh:AddVertex(Vector3.new(1, 0, 1))
	local v7 = editableMesh:AddVertex(Vector3.new(0, 1, 1))
	local v8 = editableMesh:AddVertex(Vector3.new(1, 1, 1))

	addSharpQuad(editableMesh, v5, v6, v8, v7)  -- Front
	addSharpQuad(editableMesh, v1, v3, v4, v2)  -- Back
	addSharpQuad(editableMesh, v1, v5, v7, v3)  -- Left
	addSharpQuad(editableMesh, v2, v4, v8, v6)  -- Right
	addSharpQuad(editableMesh, v1, v2, v6, v5)  -- Bottom
	addSharpQuad(editableMesh, v3, v7, v8, v4)  -- Top

	editableMesh:RemoveUnused()
	return editableMesh
end
```

#### Winding

Mesh faces have a front side and a back side. When drawing meshes, only the
front of the faces are drawn by default, although you can change this by
setting the mesh' `Class.MeshPart.DoubleSided|DoubleSided` property to `true`.

The order of the vertices around the face determines whether you are looking
at the front or the back. The front of the face is visible when the vertices
go counterclockwise around it.

<img src="../../../assets/engine-api/classes/EditableMesh/Winding.png" alt="Order of the vertices around the face" width="550" />

#### FACS poses

Animatable heads use the Facial Action Coding System (FACS). See the
[FACS poses reference](../../../avatar/dynamic-heads/facs-poses-reference.md)
for helpful information when using
`Class.EditableMesh:GetFacsPoses()|GetFacsPoses()` and similar methods.

Each FACS pose is specified by an `Enum.FacsActionUnit` value. For the FACS
pose, virtual bones can each have a `Datatype.CFrame` that transforms the
bones' initial `Datatype.CFrame` in the bind pose of the mesh into the
`Datatype.CFrame` for that FACS action unit's pose. All bone
`Datatype.CFrame|CFrames` are in the mesh's local space.

These FACS poses are blended together during animation. Sometimes, the
blending of the base poses produces poor results. In those cases, you can
override the blending of specific combinations of base poses with a
[corrective pose](../../../art/characters/facial-animation/create-basic-heads.md#combination-poses)
that is more pleasing. A corrective pose is specified by 2 or 3
`Enum.FacsActionUnit` values. Like a base FACS pose, for a corrective pose,
virtual bones can each have a `Datatype.CFrame` that transforms the bones'
initial `Datatype.CFrame` in the bind pose of the mesh into the
`Datatype.CFrame` for that FACS corrective.

Please note that corrective poses that operate on both left and right action
units are not currently expressible. For example, using `LeftCheekPuff` and
`RightEyeClosed` together in a corrective pose is not currently possible.

#### Limitations

`EditableMesh` currently has a limit of 60,000 vertices and 20,000 triangles.
Attempting to add too many vertices or triangles will cause an error.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.EditableMesh.FixedSize` | `bool` | [ReadOnly] [NotReplicated] {write: RobloxSecurity} |

## Methods

### `Class.EditableMesh:AddBone`

``AddBone(boneProperties: `Dictionary`)`` -> `int64`

### `Class.EditableMesh:AddColor`

``AddColor(color: `Datatype.Color3`, alpha: `float`)`` -> `int64`

### `Class.EditableMesh:AddFace`

``AddFace(vertexIds: `Array`)`` -> `int64`

### `Class.EditableMesh:AddNormal`

``AddNormal(normal: `Datatype.Vector3`?)`` -> `int64`

### `Class.EditableMesh:AddTriangle`

``AddTriangle(vertexId0: `int64`, vertexId1: `int64`, vertexId2: `int64`)`` -> `int64`

### `Class.EditableMesh:AddUV`

``AddUV(uv: `Datatype.Vector2`)`` -> `int64`

### `Class.EditableMesh:AddVertex`

``AddVertex(p: `Datatype.Vector3`)`` -> `int64`

### `Class.EditableMesh:Clear`

``Clear()`` -> `null`
  [NotBrowsable]

### `Class.EditableMesh:Destroy`

``Destroy()`` -> `null`

### `Class.EditableMesh:FindClosestPointOnSurface`

``FindClosestPointOnSurface(point: `Datatype.Vector3`)`` -> `Tuple`

### `Class.EditableMesh:FindClosestVertex`

``FindClosestVertex(toThisPoint: `Datatype.Vector3`)`` -> `int64`

### `Class.EditableMesh:FindVerticesWithinSphere`

``FindVerticesWithinSphere(center: `Datatype.Vector3`, radius: `float`)`` -> `Array`

### `Class.EditableMesh:GetAdjacentFaces`

``GetAdjacentFaces(faceId: `int64`)`` -> `Array`

### `Class.EditableMesh:GetAdjacentVertices`

``GetAdjacentVertices(vertexId: `int64`)`` -> `Array`

### `Class.EditableMesh:GetBoneByName`

``GetBoneByName(boneName: `string`)`` -> `int64`

### `Class.EditableMesh:GetBoneCFrame`

``GetBoneCFrame(boneId: `int64`)`` -> `Datatype.CFrame`

### `Class.EditableMesh:GetBoneIsVirtual`

``GetBoneIsVirtual(boneId: `int64`)`` -> `bool`

### `Class.EditableMesh:GetBoneName`

``GetBoneName(boneId: `int64`)`` -> `string`

### `Class.EditableMesh:GetBoneParent`

``GetBoneParent(boneId: `int64`)`` -> `int64`

### `Class.EditableMesh:GetBones`

``GetBones()`` -> `Array`

### `Class.EditableMesh:GetCenter`

``GetCenter()`` -> `Datatype.Vector3`

### `Class.EditableMesh:GetColor`

``GetColor(colorId: `int64`)`` -> `Datatype.Color3`?

### `Class.EditableMesh:GetColorAlpha`

``GetColorAlpha(colorId: `int64`)`` -> `float?`

### `Class.EditableMesh:GetColors`

``GetColors()`` -> `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetFaceColors`

``GetFaceColors(faceId: `int64`)`` -> `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetFaceNormals`

``GetFaceNormals(faceId: `int64`)`` -> `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetFaceUVs`

``GetFaceUVs(faceId: `int64`)`` -> `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetFaceVertices`

``GetFaceVertices(faceId: `int64`)`` -> `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetFaces`

``GetFaces()`` -> `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetFacesWithAttribute`

``GetFacesWithAttribute(id: `int64`)`` -> `Array`
  [Deprecated]

### `Class.EditableMesh:GetFacesWithColor`

``GetFacesWithColor(colorId: `int64`)`` -> `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetFacesWithNormal`

``GetFacesWithNormal(normalId: `int64`)`` -> `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetFacesWithUV`

``GetFacesWithUV(uvId: `int64`)`` -> `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetFacsCorrectivePose`

``GetFacsCorrectivePose(actions: `Array`)`` -> `Tuple`

### `Class.EditableMesh:GetFacsCorrectivePoses`

``GetFacsCorrectivePoses()`` -> `Array`

### `Class.EditableMesh:GetFacsPose`

``GetFacsPose(action: `Enum.FacsActionUnit`)`` -> `Tuple`

### `Class.EditableMesh:GetFacsPoses`

``GetFacsPoses()`` -> `Array`

### `Class.EditableMesh:GetNormal`

``GetNormal(normalId: `int64`)`` -> `Datatype.Vector3`?

### `Class.EditableMesh:GetNormals`

``GetNormals()`` -> `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetPosition`

``GetPosition(vertexId: `int64`)`` -> `Datatype.Vector3`

### `Class.EditableMesh:GetSize`

``GetSize()`` -> `Datatype.Vector3`

### `Class.EditableMesh:GetUV`

``GetUV(uvId: `int64`)`` -> `Datatype.Vector2`?

### `Class.EditableMesh:GetUVs`

``GetUVs()`` -> `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetVertexBoneWeights`

``GetVertexBoneWeights(vertexId: `int64`)`` -> `Array`

### `Class.EditableMesh:GetVertexBones`

``GetVertexBones(vertexId: `int64`)`` -> `Array`

### `Class.EditableMesh:GetVertexColors`

``GetVertexColors(vertexId: `int64`)`` -> `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetVertexFaceColor`

``GetVertexFaceColor(vertexId: `int64`, faceId: `int64`)`` -> `int64`

### `Class.EditableMesh:GetVertexFaceNormal`

``GetVertexFaceNormal(vertexId: `int64`, faceId: `int64`)`` -> `int64`

### `Class.EditableMesh:GetVertexFaceUV`

``GetVertexFaceUV(vertexId: `int64`, faceId: `int64`)`` -> `int64`

### `Class.EditableMesh:GetVertexFaces`

``GetVertexFaces(vertexId: `int64`)`` -> `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetVertexNormals`

``GetVertexNormals(vertexId: `int64`)`` -> `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetVertexUVs`

``GetVertexUVs(vertexId: `int64`)`` -> `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetVertices`

``GetVertices()`` -> `Array`

### `Class.EditableMesh:GetVerticesWithAttribute`

``GetVerticesWithAttribute(id: `int64`)`` -> `Array`
  [Deprecated]

### `Class.EditableMesh:GetVerticesWithColor`

``GetVerticesWithColor(colorId: `int64`)`` -> `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetVerticesWithNormal`

``GetVerticesWithNormal(normalId: `int64`)`` -> `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetVerticesWithUV`

``GetVerticesWithUV(uvId: `int64`)`` -> `Array`
  [CustomLuaState]

### `Class.EditableMesh:IdDebugString`

``IdDebugString(id: `int64`)`` -> `string`

### `Class.EditableMesh:MergeVertices`

``MergeVertices(mergeTolerance: `float`)`` -> `Map`

### `Class.EditableMesh:RaycastLocal`

``RaycastLocal(origin: `Datatype.Vector3`, direction: `Datatype.Vector3`)`` -> `Tuple`

### `Class.EditableMesh:RemoveBone`

``RemoveBone(boneId: `int64`)`` -> `null`

### `Class.EditableMesh:RemoveFace`

``RemoveFace(faceId: `int64`)`` -> `null`

### `Class.EditableMesh:RemoveUnused`

``RemoveUnused()`` -> `Array`

### `Class.EditableMesh:ResetNormal`

``ResetNormal(normalId: `int64`)`` -> `null`

### `Class.EditableMesh:SetBoneCFrame`

``SetBoneCFrame(boneId: `int64`, cframe: `Datatype.CFrame`)`` -> `null`

### `Class.EditableMesh:SetBoneIsVirtual`

``SetBoneIsVirtual(boneId: `int64`, virtual: `bool`)`` -> `null`

### `Class.EditableMesh:SetBoneName`

``SetBoneName(boneId: `int64`, name: `string`)`` -> `null`

### `Class.EditableMesh:SetBoneParent`

``SetBoneParent(boneId: `int64`, parentBoneId: `int64`)`` -> `null`

### `Class.EditableMesh:SetColor`

``SetColor(colorId: `int64`, color: `Datatype.Color3`)`` -> `null`

### `Class.EditableMesh:SetColorAlpha`

``SetColorAlpha(colorId: `int64`, alpha: `float`)`` -> `null`

### `Class.EditableMesh:SetFaceColors`

``SetFaceColors(faceId: `int64`, ids: `Array`)`` -> `null`
  [CustomLuaState]

### `Class.EditableMesh:SetFaceNormals`

``SetFaceNormals(faceId: `int64`, ids: `Array`)`` -> `null`
  [CustomLuaState]

### `Class.EditableMesh:SetFaceUVs`

``SetFaceUVs(faceId: `int64`, ids: `Array`)`` -> `null`
  [CustomLuaState]

### `Class.EditableMesh:SetFaceVertices`

``SetFaceVertices(faceId: `int64`, ids: `Array`)`` -> `null`
  [CustomLuaState]

### `Class.EditableMesh:SetFacsBonePose`

``SetFacsBonePose(action: `Enum.FacsActionUnit`, boneId: `int64`, cframe: `Datatype.CFrame`)`` -> `null`

### `Class.EditableMesh:SetFacsCorrectivePose`

``SetFacsCorrectivePose(actions: `Array`, boneIds: `Array`, cframes: `Array`)`` -> `null`

### `Class.EditableMesh:SetFacsPose`

``SetFacsPose(action: `Enum.FacsActionUnit`, boneIds: `Array`, cframes: `Array`)`` -> `null`

### `Class.EditableMesh:SetNormal`

``SetNormal(normalId: `int64`, normal: `Datatype.Vector3`)`` -> `null`

### `Class.EditableMesh:SetPosition`

``SetPosition(vertexId: `int64`, p: `Datatype.Vector3`)`` -> `null`

### `Class.EditableMesh:SetUV`

``SetUV(uvId: `int64`, uv: `Datatype.Vector2`)`` -> `null`

### `Class.EditableMesh:SetVertexBoneWeights`

``SetVertexBoneWeights(vertexId: `int64`, boneWeights: `Array`)`` -> `null`

### `Class.EditableMesh:SetVertexBones`

``SetVertexBones(vertexId: `int64`, boneIDs: `Array`)`` -> `null`

### `Class.EditableMesh:SetVertexFaceColor`

``SetVertexFaceColor(vertexId: `int64`, faceId: `int64`, colorId: `int64`)`` -> `null`

### `Class.EditableMesh:SetVertexFaceNormal`

``SetVertexFaceNormal(vertexId: `int64`, faceId: `int64`, normalId: `int64`)`` -> `null`

### `Class.EditableMesh:SetVertexFaceUV`

``SetVertexFaceUV(vertexId: `int64`, faceId: `int64`, uvId: `int64`)`` -> `null`

### `Class.EditableMesh:Triangulate`

``Triangulate()`` -> `null`

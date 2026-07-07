---
title: EditableMesh
type: class
superclass: Object
tags: [NotCreatable]
---

# EditableMesh

**Inherits from:** `Class.Object`

**Tags:** [NotCreatable]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.EditableMesh.FixedSize` | `bool` | [ReadOnly] [NotReplicated] {write: RobloxSecurity} |

## Methods

### `Class.EditableMesh:AddBone`

``AddBone(boneProperties: `Dictionary`)`` → `int64`

### `Class.EditableMesh:AddColor`

``AddColor(color: `Datatype.Color3`, alpha: `float`)`` → `int64`

### `Class.EditableMesh:AddFace`

``AddFace(vertexIds: `Array`)`` → `int64`

### `Class.EditableMesh:AddNormal`

``AddNormal(normal: `Datatype.Vector3`?)`` → `int64`

### `Class.EditableMesh:AddTriangle`

``AddTriangle(vertexId0: `int64`, vertexId1: `int64`, vertexId2: `int64`)`` → `int64`

### `Class.EditableMesh:AddUV`

``AddUV(uv: `Datatype.Vector2`)`` → `int64`

### `Class.EditableMesh:AddVertex`

``AddVertex(p: `Datatype.Vector3`)`` → `int64`

### `Class.EditableMesh:Clear`

``Clear()`` → `null`
  [NotBrowsable]

### `Class.EditableMesh:Destroy`

``Destroy()`` → `null`

### `Class.EditableMesh:FindClosestPointOnSurface`

``FindClosestPointOnSurface(point: `Datatype.Vector3`)`` → `Tuple`

### `Class.EditableMesh:FindClosestVertex`

``FindClosestVertex(toThisPoint: `Datatype.Vector3`)`` → `int64`

### `Class.EditableMesh:FindVerticesWithinSphere`

``FindVerticesWithinSphere(center: `Datatype.Vector3`, radius: `float`)`` → `Array`

### `Class.EditableMesh:GetAdjacentFaces`

``GetAdjacentFaces(faceId: `int64`)`` → `Array`

### `Class.EditableMesh:GetAdjacentVertices`

``GetAdjacentVertices(vertexId: `int64`)`` → `Array`

### `Class.EditableMesh:GetBoneByName`

``GetBoneByName(boneName: `string`)`` → `int64`

### `Class.EditableMesh:GetBoneCFrame`

``GetBoneCFrame(boneId: `int64`)`` → `Datatype.CFrame`

### `Class.EditableMesh:GetBoneIsVirtual`

``GetBoneIsVirtual(boneId: `int64`)`` → `bool`

### `Class.EditableMesh:GetBoneName`

``GetBoneName(boneId: `int64`)`` → `string`

### `Class.EditableMesh:GetBoneParent`

``GetBoneParent(boneId: `int64`)`` → `int64`

### `Class.EditableMesh:GetBones`

``GetBones()`` → `Array`

### `Class.EditableMesh:GetCenter`

``GetCenter()`` → `Datatype.Vector3`

### `Class.EditableMesh:GetColor`

``GetColor(colorId: `int64`)`` → `Datatype.Color3`?

### `Class.EditableMesh:GetColorAlpha`

``GetColorAlpha(colorId: `int64`)`` → `float?`

### `Class.EditableMesh:GetColors`

``GetColors()`` → `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetFaceColors`

``GetFaceColors(faceId: `int64`)`` → `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetFaceNormals`

``GetFaceNormals(faceId: `int64`)`` → `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetFaceUVs`

``GetFaceUVs(faceId: `int64`)`` → `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetFaceVertices`

``GetFaceVertices(faceId: `int64`)`` → `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetFaces`

``GetFaces()`` → `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetFacesWithAttribute`

``GetFacesWithAttribute(id: `int64`)`` → `Array`
  [Deprecated]

### `Class.EditableMesh:GetFacesWithColor`

``GetFacesWithColor(colorId: `int64`)`` → `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetFacesWithNormal`

``GetFacesWithNormal(normalId: `int64`)`` → `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetFacesWithUV`

``GetFacesWithUV(uvId: `int64`)`` → `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetFacsCorrectivePose`

``GetFacsCorrectivePose(actions: `Array`)`` → `Tuple`

### `Class.EditableMesh:GetFacsCorrectivePoses`

``GetFacsCorrectivePoses()`` → `Array`

### `Class.EditableMesh:GetFacsPose`

``GetFacsPose(action: `Enum.FacsActionUnit`)`` → `Tuple`

### `Class.EditableMesh:GetFacsPoses`

``GetFacsPoses()`` → `Array`

### `Class.EditableMesh:GetNormal`

``GetNormal(normalId: `int64`)`` → `Datatype.Vector3`?

### `Class.EditableMesh:GetNormals`

``GetNormals()`` → `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetPosition`

``GetPosition(vertexId: `int64`)`` → `Datatype.Vector3`

### `Class.EditableMesh:GetSize`

``GetSize()`` → `Datatype.Vector3`

### `Class.EditableMesh:GetUV`

``GetUV(uvId: `int64`)`` → `Datatype.Vector2`?

### `Class.EditableMesh:GetUVs`

``GetUVs()`` → `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetVertexBoneWeights`

``GetVertexBoneWeights(vertexId: `int64`)`` → `Array`

### `Class.EditableMesh:GetVertexBones`

``GetVertexBones(vertexId: `int64`)`` → `Array`

### `Class.EditableMesh:GetVertexColors`

``GetVertexColors(vertexId: `int64`)`` → `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetVertexFaceColor`

``GetVertexFaceColor(vertexId: `int64`, faceId: `int64`)`` → `int64`

### `Class.EditableMesh:GetVertexFaceNormal`

``GetVertexFaceNormal(vertexId: `int64`, faceId: `int64`)`` → `int64`

### `Class.EditableMesh:GetVertexFaceUV`

``GetVertexFaceUV(vertexId: `int64`, faceId: `int64`)`` → `int64`

### `Class.EditableMesh:GetVertexFaces`

``GetVertexFaces(vertexId: `int64`)`` → `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetVertexNormals`

``GetVertexNormals(vertexId: `int64`)`` → `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetVertexUVs`

``GetVertexUVs(vertexId: `int64`)`` → `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetVertices`

``GetVertices()`` → `Array`

### `Class.EditableMesh:GetVerticesWithAttribute`

``GetVerticesWithAttribute(id: `int64`)`` → `Array`
  [Deprecated]

### `Class.EditableMesh:GetVerticesWithColor`

``GetVerticesWithColor(colorId: `int64`)`` → `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetVerticesWithNormal`

``GetVerticesWithNormal(normalId: `int64`)`` → `Array`
  [CustomLuaState]

### `Class.EditableMesh:GetVerticesWithUV`

``GetVerticesWithUV(uvId: `int64`)`` → `Array`
  [CustomLuaState]

### `Class.EditableMesh:IdDebugString`

``IdDebugString(id: `int64`)`` → `string`

### `Class.EditableMesh:MergeVertices`

``MergeVertices(mergeTolerance: `float`)`` → `Map`

### `Class.EditableMesh:RaycastLocal`

``RaycastLocal(origin: `Datatype.Vector3`, direction: `Datatype.Vector3`)`` → `Tuple`

### `Class.EditableMesh:RemoveBone`

``RemoveBone(boneId: `int64`)`` → `null`

### `Class.EditableMesh:RemoveFace`

``RemoveFace(faceId: `int64`)`` → `null`

### `Class.EditableMesh:RemoveUnused`

``RemoveUnused()`` → `Array`

### `Class.EditableMesh:ResetNormal`

``ResetNormal(normalId: `int64`)`` → `null`

### `Class.EditableMesh:SetBoneCFrame`

``SetBoneCFrame(boneId: `int64`, cframe: `Datatype.CFrame`)`` → `null`

### `Class.EditableMesh:SetBoneIsVirtual`

``SetBoneIsVirtual(boneId: `int64`, virtual: `bool`)`` → `null`

### `Class.EditableMesh:SetBoneName`

``SetBoneName(boneId: `int64`, name: `string`)`` → `null`

### `Class.EditableMesh:SetBoneParent`

``SetBoneParent(boneId: `int64`, parentBoneId: `int64`)`` → `null`

### `Class.EditableMesh:SetColor`

``SetColor(colorId: `int64`, color: `Datatype.Color3`)`` → `null`

### `Class.EditableMesh:SetColorAlpha`

``SetColorAlpha(colorId: `int64`, alpha: `float`)`` → `null`

### `Class.EditableMesh:SetFaceColors`

``SetFaceColors(faceId: `int64`, ids: `Array`)`` → `null`
  [CustomLuaState]

### `Class.EditableMesh:SetFaceNormals`

``SetFaceNormals(faceId: `int64`, ids: `Array`)`` → `null`
  [CustomLuaState]

### `Class.EditableMesh:SetFaceUVs`

``SetFaceUVs(faceId: `int64`, ids: `Array`)`` → `null`
  [CustomLuaState]

### `Class.EditableMesh:SetFaceVertices`

``SetFaceVertices(faceId: `int64`, ids: `Array`)`` → `null`
  [CustomLuaState]

### `Class.EditableMesh:SetFacsBonePose`

``SetFacsBonePose(action: `Enum.FacsActionUnit`, boneId: `int64`, cframe: `Datatype.CFrame`)`` → `null`

### `Class.EditableMesh:SetFacsCorrectivePose`

``SetFacsCorrectivePose(actions: `Array`, boneIds: `Array`, cframes: `Array`)`` → `null`

### `Class.EditableMesh:SetFacsPose`

``SetFacsPose(action: `Enum.FacsActionUnit`, boneIds: `Array`, cframes: `Array`)`` → `null`

### `Class.EditableMesh:SetNormal`

``SetNormal(normalId: `int64`, normal: `Datatype.Vector3`)`` → `null`

### `Class.EditableMesh:SetPosition`

``SetPosition(vertexId: `int64`, p: `Datatype.Vector3`)`` → `null`

### `Class.EditableMesh:SetUV`

``SetUV(uvId: `int64`, uv: `Datatype.Vector2`)`` → `null`

### `Class.EditableMesh:SetVertexBoneWeights`

``SetVertexBoneWeights(vertexId: `int64`, boneWeights: `Array`)`` → `null`

### `Class.EditableMesh:SetVertexBones`

``SetVertexBones(vertexId: `int64`, boneIDs: `Array`)`` → `null`

### `Class.EditableMesh:SetVertexFaceColor`

``SetVertexFaceColor(vertexId: `int64`, faceId: `int64`, colorId: `int64`)`` → `null`

### `Class.EditableMesh:SetVertexFaceNormal`

``SetVertexFaceNormal(vertexId: `int64`, faceId: `int64`, normalId: `int64`)`` → `null`

### `Class.EditableMesh:SetVertexFaceUV`

``SetVertexFaceUV(vertexId: `int64`, faceId: `int64`, uvId: `int64`)`` → `null`

### `Class.EditableMesh:Triangulate`

``Triangulate()`` → `null`

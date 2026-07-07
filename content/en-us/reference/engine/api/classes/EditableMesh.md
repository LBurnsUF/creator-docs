---
title: EditableMesh
type: class
superclass: Object
tags: [NotCreatable]
---

# EditableMesh

**Inherits**: Object

**Tags**: NotCreatable

## Properties

- **FixedSize**: `bool` [ReadOnly] [NotReplicated] (Security: Read=None, Write=RobloxSecurity)

## Methods

- **AddBone**(`boneProperties: Dictionary`) -> `int64`
- **AddColor**(`color: Color3`, `alpha: float`) -> `int64`
- **AddFace**(`vertexIds: Array`) -> `int64`
- **AddNormal**(`normal: Vector3?`) -> `int64`
- **AddTriangle**(`vertexId0: int64`, `vertexId1: int64`, `vertexId2: int64`) -> `int64`
- **AddUV**(`uv: Vector2`) -> `int64`
- **AddVertex**(`p: Vector3`) -> `int64`
- **Clear**() -> `null` [NotBrowsable]
- **Destroy**() -> `null`
- **FindClosestPointOnSurface**(`point: Vector3`) -> `Tuple`
- **FindClosestVertex**(`toThisPoint: Vector3`) -> `int64`
- **FindVerticesWithinSphere**(`center: Vector3`, `radius: float`) -> `Array`
- **GetAdjacentFaces**(`faceId: int64`) -> `Array`
- **GetAdjacentVertices**(`vertexId: int64`) -> `Array`
- **GetBoneByName**(`boneName: string`) -> `int64`
- **GetBoneCFrame**(`boneId: int64`) -> `CFrame`
- **GetBoneIsVirtual**(`boneId: int64`) -> `bool`
- **GetBoneName**(`boneId: int64`) -> `string`
- **GetBoneParent**(`boneId: int64`) -> `int64`
- **GetBones**() -> `Array`
- **GetCenter**() -> `Vector3`
- **GetColor**(`colorId: int64`) -> `Color3?`
- **GetColorAlpha**(`colorId: int64`) -> `float?`
- **GetColors**() -> `Array` [CustomLuaState]
- **GetFaceColors**(`faceId: int64`) -> `Array` [CustomLuaState]
- **GetFaceNormals**(`faceId: int64`) -> `Array` [CustomLuaState]
- **GetFaceUVs**(`faceId: int64`) -> `Array` [CustomLuaState]
- **GetFaceVertices**(`faceId: int64`) -> `Array` [CustomLuaState]
- **GetFaces**() -> `Array` [CustomLuaState]
- **GetFacesWithAttribute**(`id: int64`) -> `Array` [Deprecated]
- **GetFacesWithColor**(`colorId: int64`) -> `Array` [CustomLuaState]
- **GetFacesWithNormal**(`normalId: int64`) -> `Array` [CustomLuaState]
- **GetFacesWithUV**(`uvId: int64`) -> `Array` [CustomLuaState]
- **GetFacsCorrectivePose**(`actions: Array`) -> `Tuple`
- **GetFacsCorrectivePoses**() -> `Array`
- **GetFacsPose**(`action: FacsActionUnit`) -> `Tuple`
- **GetFacsPoses**() -> `Array`
- **GetNormal**(`normalId: int64`) -> `Vector3?`
- **GetNormals**() -> `Array` [CustomLuaState]
- **GetPosition**(`vertexId: int64`) -> `Vector3`
- **GetSize**() -> `Vector3`
- **GetUV**(`uvId: int64`) -> `Vector2?`
- **GetUVs**() -> `Array` [CustomLuaState]
- **GetVertexBoneWeights**(`vertexId: int64`) -> `Array`
- **GetVertexBones**(`vertexId: int64`) -> `Array`
- **GetVertexColors**(`vertexId: int64`) -> `Array` [CustomLuaState]
- **GetVertexFaceColor**(`vertexId: int64`, `faceId: int64`) -> `int64`
- **GetVertexFaceNormal**(`vertexId: int64`, `faceId: int64`) -> `int64`
- **GetVertexFaceUV**(`vertexId: int64`, `faceId: int64`) -> `int64`
- **GetVertexFaces**(`vertexId: int64`) -> `Array` [CustomLuaState]
- **GetVertexNormals**(`vertexId: int64`) -> `Array` [CustomLuaState]
- **GetVertexUVs**(`vertexId: int64`) -> `Array` [CustomLuaState]
- **GetVertices**() -> `Array`
- **GetVerticesWithAttribute**(`id: int64`) -> `Array` [Deprecated]
- **GetVerticesWithColor**(`colorId: int64`) -> `Array` [CustomLuaState]
- **GetVerticesWithNormal**(`normalId: int64`) -> `Array` [CustomLuaState]
- **GetVerticesWithUV**(`uvId: int64`) -> `Array` [CustomLuaState]
- **IdDebugString**(`id: int64`) -> `string`
- **MergeVertices**(`mergeTolerance: float`) -> `Map`
- **RaycastLocal**(`origin: Vector3`, `direction: Vector3`) -> `Tuple`
- **RemoveBone**(`boneId: int64`) -> `null`
- **RemoveFace**(`faceId: int64`) -> `null`
- **RemoveUnused**() -> `Array`
- **ResetNormal**(`normalId: int64`) -> `null`
- **SetBoneCFrame**(`boneId: int64`, `cframe: CFrame`) -> `null`
- **SetBoneIsVirtual**(`boneId: int64`, `virtual: bool`) -> `null`
- **SetBoneName**(`boneId: int64`, `name: string`) -> `null`
- **SetBoneParent**(`boneId: int64`, `parentBoneId: int64`) -> `null`
- **SetColor**(`colorId: int64`, `color: Color3`) -> `null`
- **SetColorAlpha**(`colorId: int64`, `alpha: float`) -> `null`
- **SetFaceColors**(`faceId: int64`, `ids: Array`) -> `null` [CustomLuaState]
- **SetFaceNormals**(`faceId: int64`, `ids: Array`) -> `null` [CustomLuaState]
- **SetFaceUVs**(`faceId: int64`, `ids: Array`) -> `null` [CustomLuaState]
- **SetFaceVertices**(`faceId: int64`, `ids: Array`) -> `null` [CustomLuaState]
- **SetFacsBonePose**(`action: FacsActionUnit`, `boneId: int64`, `cframe: CFrame`) -> `null`
- **SetFacsCorrectivePose**(`actions: Array`, `boneIds: Array`, `cframes: Array`) -> `null`
- **SetFacsPose**(`action: FacsActionUnit`, `boneIds: Array`, `cframes: Array`) -> `null`
- **SetNormal**(`normalId: int64`, `normal: Vector3`) -> `null`
- **SetPosition**(`vertexId: int64`, `p: Vector3`) -> `null`
- **SetUV**(`uvId: int64`, `uv: Vector2`) -> `null`
- **SetVertexBoneWeights**(`vertexId: int64`, `boneWeights: Array`) -> `null`
- **SetVertexBones**(`vertexId: int64`, `boneIDs: Array`) -> `null`
- **SetVertexFaceColor**(`vertexId: int64`, `faceId: int64`, `colorId: int64`) -> `null`
- **SetVertexFaceNormal**(`vertexId: int64`, `faceId: int64`, `normalId: int64`) -> `null`
- **SetVertexFaceUV**(`vertexId: int64`, `faceId: int64`, `uvId: int64`) -> `null`
- **Triangulate**() -> `null`

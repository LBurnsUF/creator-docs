---
title: UGCValidationService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# UGCValidationService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.UGCValidationService:CalculateAverageEditableCageMeshDistance`

``CalculateAverageEditableCageMeshDistance(innerCage: `Class.EditableMesh`, outerCage: `Class.EditableMesh`, refMesh: `Class.EditableMesh`, innerTransform: `Datatype.CFrame`, outerTransform: `Datatype.CFrame`)`` -> `float`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:CalculateBodyMaxCageDistance`

``CalculateBodyMaxCageDistance(inputBodyParts: `Array`)`` -> `Tuple`
  [Yields] {security: RobloxScriptSecurity}

### `Class.UGCValidationService:CalculateEditableMeshInsideMeshPercentage`

``CalculateEditableMeshInsideMeshPercentage(editableMeshRoot: `Class.EditableMesh`, editableMeshQuery: `Class.EditableMesh`, meshQueryTransform: `Datatype.CFrame`, meshQueryScale: `Datatype.Vector3`)`` -> `float`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:CalculateEditableMeshModifiedCageBoundingBox`

``CalculateEditableMeshModifiedCageBoundingBox(referenceUVValues: `Array`, innerCage: `Class.EditableMesh`, innerTransform: `Datatype.CFrame`, outerCage: `Class.EditableMesh`, outerTransform: `Datatype.CFrame`)`` -> `Tuple`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:CalculateEditableMeshNumModifiedCageUVsInSet`

``CalculateEditableMeshNumModifiedCageUVsInSet(referenceUVValues: `Array`, innerCage: `Class.EditableMesh`, innerTransform: `Datatype.CFrame`, outerCage: `Class.EditableMesh`, outerTransform: `Datatype.CFrame`)`` -> `Tuple`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:CalculateEditableMeshTotalSurfaceArea`

``CalculateEditableMeshTotalSurfaceArea(editableMesh: `Class.EditableMesh`, meshScale: `Datatype.Vector3`)`` -> `float`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:CalculateEditableMeshUniqueUVCount`

``CalculateEditableMeshUniqueUVCount(editableMesh: `Class.EditableMesh`)`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:CanLoadAsset`

``CanLoadAsset(assetId: `string`)`` -> `bool`
  [Yields] {security: RobloxScriptSecurity}

### `Class.UGCValidationService:CheckEditableMeshInCameraFrustum`

``CheckEditableMeshInCameraFrustum(editableMesh: `Class.EditableMesh`, meshScale: `Datatype.Vector3`, handleWorldCF: `Datatype.CFrame`, cameraWorldCF: `Datatype.CFrame`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:CreateEditableImageFromBinaryStringRobloxOnly`

``CreateEditableImageFromBinaryStringRobloxOnly(value: `Class.BinaryStringValue`)`` -> `Class.EditableImage`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:CreateEditableImageOriginalSizeAsync`

``CreateEditableImageOriginalSizeAsync(textureId: `string`)`` -> `Class.EditableImage`
  [Yields] {security: RobloxScriptSecurity}

### `Class.UGCValidationService:CreateEditableMeshFromBinaryStringRobloxOnly`

``CreateEditableMeshFromBinaryStringRobloxOnly(value: `Class.BinaryStringValue`)`` -> `Class.EditableMesh`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:DoesMeshHaveSkinningData`

``DoesMeshHaveSkinningData(meshId: `string`)`` -> `bool`
  [Yields] {security: RobloxScriptSecurity}

### `Class.UGCValidationService:DoesSurfaceAppearanceMatchTexturePackAsync`

``DoesSurfaceAppearanceMatchTexturePackAsync(surfaceAppearance: `Class.SurfaceAppearance`)`` -> `bool`
  [Yields] {security: RobloxScriptSecurity}

### `Class.UGCValidationService:FetchAssetWithFormat`

``FetchAssetWithFormat(url: `Datatype.ContentId`, assetFormat: `string`)`` -> `Datatype.Instances`
  [Yields] {security: RobloxScriptSecurity}

### `Class.UGCValidationService:GetBoundingBoxManipulationData`

``GetBoundingBoxManipulationData(partMeshObjects: `Array`, partCFs: `Array`, meshScales: `Array`)`` -> `Map`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:GetDynamicHeadEditableMeshInactiveControls`

``GetDynamicHeadEditableMeshInactiveControls(editableMesh: `Class.EditableMesh`, controlNames: `Array`)`` -> `Tuple`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:GetEditableCagingRelevancyMetrics`

``GetEditableCagingRelevancyMetrics(innerCage: `Class.EditableMesh`, outerCage: `Class.EditableMesh`, refMesh: `Class.EditableMesh`, offsetInner: `Datatype.Vector3`, offsetOuter: `Datatype.Vector3`)`` -> `Tuple`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:GetEditableImageSize`

``GetEditableImageSize(editableImage: `Class.EditableImage`)`` -> `Datatype.Vector2`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:GetEditableMeshMaxNearbyVerticesCollisions`

``GetEditableMeshMaxNearbyVerticesCollisions(editableMesh: `Class.EditableMesh`, meshScale: `Datatype.Vector3`)`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:GetEditableMeshSkinningTransferJointsInfo`

``GetEditableMeshSkinningTransferJointsInfo(editableMesh: `Class.EditableMesh`)`` -> `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:GetEditableMeshTriCount`

``GetEditableMeshTriCount(editableMesh: `Class.EditableMesh`)`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:GetEditableMeshVertColors`

``GetEditableMeshVertColors(editableMesh: `Class.EditableMesh`)`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:GetEditableMeshVerticesSimilarityRate`

``GetEditableMeshVerticesSimilarityRate(editableMesh: `Class.EditableMesh`, meshScale: `Datatype.Vector3`)`` -> `float`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:GetEditableMeshVerts`

``GetEditableMeshVerts(editableMesh: `Class.EditableMesh`)`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:GetExpectedTposeRotation`

``GetExpectedTposeRotation(jointLabel: `Enum.RigLabel`, partsFolder: `Class.Instance`)`` -> `Datatype.CFrame`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:GetFacsDrivenJointNamesFromEditableMesh`

``GetFacsDrivenJointNamesFromEditableMesh(editableMesh: `Class.EditableMesh`)`` -> `Tuple`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:GetLayeredClothingPostDeformationSize`

``GetLayeredClothingPostDeformationSize(accessory: `Class.Accessory`, editableMesh: `Class.EditableMesh`, meshScale: `Datatype.Vector3`)`` -> `Datatype.Vector3`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:GetMaximalJointDistancesWithinFacs`

``GetMaximalJointDistancesWithinFacs(editableMesh: `Class.EditableMesh`)`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:GetMeshDataBinaryString`

``GetMeshDataBinaryString(meshId: `string`)`` -> `Class.BinaryStringValue`
  [Yields] {security: RobloxScriptSecurity}

### `Class.UGCValidationService:GetMeshVerts`

``GetMeshVerts(meshId: `string`)`` -> `Array`
  [Yields] {security: RobloxScriptSecurity}

### `Class.UGCValidationService:GetMinAndMaxMeshSizeAcrossAllFacs`

``GetMinAndMaxMeshSizeAcrossAllFacs(editableMesh: `Class.EditableMesh`)`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:GetPropertyValue`

``GetPropertyValue(instance: `Class.Instance`, property: `string`)`` -> `Variant`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:GetSkinnedJointNamesFromEditableMesh`

``GetSkinnedJointNamesFromEditableMesh(editableMesh: `Class.EditableMesh`)`` -> `Tuple`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:IsDeformedLayeredClothingOutOfRenderBounds`

``IsDeformedLayeredClothingOutOfRenderBounds(accessory: `Class.Accessory`)`` -> `bool`
  [Yields] {security: RobloxScriptSecurity}

### `Class.UGCValidationService:IsEditableMeshNumCoplanarIntersectionsOverLimit`

``IsEditableMeshNumCoplanarIntersectionsOverLimit(editableMesh: `Class.EditableMesh`, limit: `int`, meshScale: `Datatype.Vector3`, intersectBackFaces: `bool`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:RegisterAlternateMesh`

``RegisterAlternateMesh(alternateId: `string`, binaryStringValue: `Class.BinaryStringValue`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:RegisterUGCValidationFunction`

``RegisterUGCValidationFunction(setFunction: `Datatype.Function`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ReportUGCValidationCounter`

``ReportUGCValidationCounter(success: `bool`, validationType: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ReportUGCValidationFailureTelemetry`

``ReportUGCValidationFailureTelemetry(errorType: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ReportUGCValidationTelemetry`

``ReportUGCValidationTelemetry(assetType: `string`, data: `Dictionary`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ResetCollisionFidelity`

``ResetCollisionFidelity(meshPart: `Class.Instance`, collisionFidelity: `Enum.CollisionFidelity`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ResetCollisionFidelityWithEditableMeshDataLua`

``ResetCollisionFidelityWithEditableMeshDataLua(meshPart: `Class.MeshPart`, editableMesh: `Class.EditableMesh`, collisionFidelity: `Enum.CollisionFidelity`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:SetMeshIdBlocking`

``SetMeshIdBlocking(meshPart: `Class.Instance`, meshId: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidateDynamicHeadEditableMesh`

``ValidateDynamicHeadEditableMesh(editableMesh: `Class.EditableMesh`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidateEditableMeshCageMeshIntersection`

``ValidateEditableMeshCageMeshIntersection(innerCage: `Class.EditableMesh`, outerCage: `Class.EditableMesh`, refMesh: `Class.EditableMesh`)`` -> `Tuple`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidateEditableMeshCageNonManifoldAndHoles`

``ValidateEditableMeshCageNonManifoldAndHoles(editableMesh: `Class.EditableMesh`)`` -> `Tuple`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidateEditableMeshCageUVCoincident`

``ValidateEditableMeshCageUVCoincident(editableMesh: `Class.EditableMesh`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidateEditableMeshCageUVTriangleArea`

``ValidateEditableMeshCageUVTriangleArea(editableMesh: `Class.EditableMesh`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidateEditableMeshFacialBounds`

``ValidateEditableMeshFacialBounds(editableMesh: `Class.EditableMesh`, boundsScale: `float`, partSize: `Datatype.Vector3`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidateEditableMeshFacialExpressiveness`

``ValidateEditableMeshFacialExpressiveness(editableMesh: `Class.EditableMesh`, minDelta: `float`, partSize: `Datatype.Vector3`)`` -> `float`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidateEditableMeshFullBodyCageDeletion`

``ValidateEditableMeshFullBodyCageDeletion(editableMesh: `Class.EditableMesh`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidateEditableMeshMisMatchUV`

``ValidateEditableMeshMisMatchUV(innerCage: `Class.EditableMesh`, outerCage: `Class.EditableMesh`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidateEditableMeshOverlappingVertices`

``ValidateEditableMeshOverlappingVertices(editableMesh: `Class.EditableMesh`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidateEditableMeshTriangleArea`

``ValidateEditableMeshTriangleArea(editableMesh: `Class.EditableMesh`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidateEditableMeshTriangles`

``ValidateEditableMeshTriangles(editableMesh: `Class.EditableMesh`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidateEditableMeshUVDuplicates`

``ValidateEditableMeshUVDuplicates(referenceValues: `Array`, editableMesh: `Class.EditableMesh`)`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidateEditableMeshUVSpace`

``ValidateEditableMeshUVSpace(editableMesh: `Class.EditableMesh`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidateEditableMeshUVValuesInReference`

``ValidateEditableMeshUVValuesInReference(referenceValues: `Array`, editableMesh: `Class.EditableMesh`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidateEditableMeshUniqueUVCount`

``ValidateEditableMeshUniqueUVCount(editableMesh: `Class.EditableMesh`, numRequired: `int`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidateEditableMeshVertColors`

``ValidateEditableMeshVertColors(editableMesh: `Class.EditableMesh`, includeAlpha: `bool`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidateHSRMeshIds`

``ValidateHSRMeshIds(wrapLayerInstance: `Class.Instance`, hsrInstance: `Class.Instance`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidateLeaderSkinnedVertsNearCageIslands`

``ValidateLeaderSkinnedVertsNearCageIslands(renderMesh: `Class.EditableMesh`, innerCage: `Class.EditableMesh`, cageUVs: `Array`, referenceOrigin: `Datatype.CFrame`, distanceThreshold: `float`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidatePartBBoxAfterFullFacs`

``ValidatePartBBoxAfterFullFacs(headEditableMesh: `Class.EditableMesh`, partEditableMesh: `Class.EditableMesh`, headScale: `Datatype.Vector3`, partScale: `Datatype.Vector3`, boundsMaxMultiplier: `float`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidatePropertiesSensible`

``ValidatePropertiesSensible(instance: `Class.Instance`, stringLenRestrictions: `Dictionary`)`` -> `Tuple`
   {security: RobloxScriptSecurity}

### `Class.UGCValidationService:ValidateSkinnedEditableMesh`

``ValidateSkinnedEditableMesh(editableMesh: `Class.EditableMesh`)`` -> `bool`
   {security: RobloxScriptSecurity}

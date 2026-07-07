---
title: UGCValidationService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# UGCValidationService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **CalculateAverageEditableCageMeshDistance**(`innerCage: EditableMesh`, `outerCage: EditableMesh`, `refMesh: EditableMesh`, `innerTransform: CFrame`, `outerTransform: CFrame`) -> `float`
- **CalculateBodyMaxCageDistance**(`inputBodyParts: Array`) -> `Tuple` [Yields]
- **CalculateEditableMeshInsideMeshPercentage**(`editableMeshRoot: EditableMesh`, `editableMeshQuery: EditableMesh`, `meshQueryTransform: CFrame`, `meshQueryScale: Vector3`) -> `float`
- **CalculateEditableMeshModifiedCageBoundingBox**(`referenceUVValues: Array`, `innerCage: EditableMesh`, `innerTransform: CFrame`, `outerCage: EditableMesh`, `outerTransform: CFrame`) -> `Tuple`
- **CalculateEditableMeshNumModifiedCageUVsInSet**(`referenceUVValues: Array`, `innerCage: EditableMesh`, `innerTransform: CFrame`, `outerCage: EditableMesh`, `outerTransform: CFrame`) -> `Tuple`
- **CalculateEditableMeshTotalSurfaceArea**(`editableMesh: EditableMesh`, `meshScale: Vector3`) -> `float`
- **CalculateEditableMeshUniqueUVCount**(`editableMesh: EditableMesh`) -> `int`
- **CanLoadAsset**(`assetId: string`) -> `bool` [Yields]
- **CheckEditableMeshInCameraFrustum**(`editableMesh: EditableMesh`, `meshScale: Vector3`, `handleWorldCF: CFrame`, `cameraWorldCF: CFrame`) -> `bool`
- **CreateEditableImageFromBinaryStringRobloxOnly**(`value: BinaryStringValue`) -> `EditableImage`
- **CreateEditableImageOriginalSizeAsync**(`textureId: string`) -> `EditableImage` [Yields]
- **CreateEditableMeshFromBinaryStringRobloxOnly**(`value: BinaryStringValue`) -> `EditableMesh`
- **DoesMeshHaveSkinningData**(`meshId: string`) -> `bool` [Yields]
- **DoesSurfaceAppearanceMatchTexturePackAsync**(`surfaceAppearance: SurfaceAppearance`) -> `bool` [Yields]
- **FetchAssetWithFormat**(`url: ContentId`, `assetFormat: string`) -> `Instances` [Yields]
- **GetBoundingBoxManipulationData**(`partMeshObjects: Array`, `partCFs: Array`, `meshScales: Array`) -> `Map`
- **GetDynamicHeadEditableMeshInactiveControls**(`editableMesh: EditableMesh`, `controlNames: Array`) -> `Tuple`
- **GetEditableCagingRelevancyMetrics**(`innerCage: EditableMesh`, `outerCage: EditableMesh`, `refMesh: EditableMesh`, `offsetInner: Vector3`, `offsetOuter: Vector3`) -> `Tuple`
- **GetEditableImageSize**(`editableImage: EditableImage`) -> `Vector2`
- **GetEditableMeshMaxNearbyVerticesCollisions**(`editableMesh: EditableMesh`, `meshScale: Vector3`) -> `int`
- **GetEditableMeshSkinningTransferJointsInfo**(`editableMesh: EditableMesh`) -> `Dictionary`
- **GetEditableMeshTriCount**(`editableMesh: EditableMesh`) -> `int`
- **GetEditableMeshVertColors**(`editableMesh: EditableMesh`) -> `Array`
- **GetEditableMeshVerticesSimilarityRate**(`editableMesh: EditableMesh`, `meshScale: Vector3`) -> `float`
- **GetEditableMeshVerts**(`editableMesh: EditableMesh`) -> `Array`
- **GetExpectedTposeRotation**(`jointLabel: RigLabel`, `partsFolder: Instance`) -> `CFrame`
- **GetFacsDrivenJointNamesFromEditableMesh**(`editableMesh: EditableMesh`) -> `Tuple`
- **GetLayeredClothingPostDeformationSize**(`accessory: Accessory`, `editableMesh: EditableMesh`, `meshScale: Vector3`) -> `Vector3`
- **GetMaximalJointDistancesWithinFacs**(`editableMesh: EditableMesh`) -> `Array`
- **GetMeshDataBinaryString**(`meshId: string`) -> `BinaryStringValue` [Yields]
- **GetMeshVerts**(`meshId: string`) -> `Array` [Yields]
- **GetMinAndMaxMeshSizeAcrossAllFacs**(`editableMesh: EditableMesh`) -> `Array`
- **GetPropertyValue**(`instance: Instance`, `property: string`) -> `Variant`
- **GetSkinnedJointNamesFromEditableMesh**(`editableMesh: EditableMesh`) -> `Tuple`
- **IsDeformedLayeredClothingOutOfRenderBounds**(`accessory: Accessory`) -> `bool` [Yields]
- **IsEditableMeshNumCoplanarIntersectionsOverLimit**(`editableMesh: EditableMesh`, `limit: int`, `meshScale: Vector3`, `intersectBackFaces: bool`) -> `bool`
- **RegisterAlternateMesh**(`alternateId: string`, `binaryStringValue: BinaryStringValue`) -> `null`
- **RegisterUGCValidationFunction**(`setFunction: Function`) -> `null`
- **ReportUGCValidationCounter**(`success: bool`, `validationType: string`) -> `null`
- **ReportUGCValidationFailureTelemetry**(`errorType: string`) -> `null`
- **ReportUGCValidationTelemetry**(`assetType: string`, `data: Dictionary`) -> `null`
- **ResetCollisionFidelity**(`meshPart: Instance`, `collisionFidelity: CollisionFidelity = Box`) -> `null`
- **ResetCollisionFidelityWithEditableMeshDataLua**(`meshPart: MeshPart`, `editableMesh: EditableMesh`, `collisionFidelity: CollisionFidelity = Box`) -> `null`
- **SetMeshIdBlocking**(`meshPart: Instance`, `meshId: string`) -> `null`
- **ValidateDynamicHeadEditableMesh**(`editableMesh: EditableMesh`) -> `bool`
- **ValidateEditableMeshCageMeshIntersection**(`innerCage: EditableMesh`, `outerCage: EditableMesh`, `refMesh: EditableMesh`) -> `Tuple`
- **ValidateEditableMeshCageNonManifoldAndHoles**(`editableMesh: EditableMesh`) -> `Tuple`
- **ValidateEditableMeshCageUVCoincident**(`editableMesh: EditableMesh`) -> `bool`
- **ValidateEditableMeshCageUVTriangleArea**(`editableMesh: EditableMesh`) -> `bool`
- **ValidateEditableMeshFacialBounds**(`editableMesh: EditableMesh`, `boundsScale: float`, `partSize: Vector3`) -> `bool`
- **ValidateEditableMeshFacialExpressiveness**(`editableMesh: EditableMesh`, `minDelta: float`, `partSize: Vector3`) -> `float`
- **ValidateEditableMeshFullBodyCageDeletion**(`editableMesh: EditableMesh`) -> `bool`
- **ValidateEditableMeshMisMatchUV**(`innerCage: EditableMesh`, `outerCage: EditableMesh`) -> `bool`
- **ValidateEditableMeshOverlappingVertices**(`editableMesh: EditableMesh`) -> `bool`
- **ValidateEditableMeshTriangleArea**(`editableMesh: EditableMesh`) -> `bool`
- **ValidateEditableMeshTriangles**(`editableMesh: EditableMesh`) -> `bool`
- **ValidateEditableMeshUVDuplicates**(`referenceValues: Array`, `editableMesh: EditableMesh`) -> `int`
- **ValidateEditableMeshUVSpace**(`editableMesh: EditableMesh`) -> `bool`
- **ValidateEditableMeshUVValuesInReference**(`referenceValues: Array`, `editableMesh: EditableMesh`) -> `bool`
- **ValidateEditableMeshUniqueUVCount**(`editableMesh: EditableMesh`, `numRequired: int`) -> `bool`
- **ValidateEditableMeshVertColors**(`editableMesh: EditableMesh`, `includeAlpha: bool = true`) -> `bool`
- **ValidateHSRMeshIds**(`wrapLayerInstance: Instance`, `hsrInstance: Instance`) -> `bool`
- **ValidateLeaderSkinnedVertsNearCageIslands**(`renderMesh: EditableMesh`, `innerCage: EditableMesh`, `cageUVs: Array`, `referenceOrigin: CFrame`, `distanceThreshold: float`) -> `bool`
- **ValidatePartBBoxAfterFullFacs**(`headEditableMesh: EditableMesh`, `partEditableMesh: EditableMesh`, `headScale: Vector3`, `partScale: Vector3`, `boundsMaxMultiplier: float`) -> `bool`
- **ValidatePropertiesSensible**(`instance: Instance`, `stringLenRestrictions: Dictionary = nil`) -> `Tuple`
- **ValidateSkinnedEditableMesh**(`editableMesh: EditableMesh`) -> `bool`

---
title: AssetService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# AssetService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **AllowInsertFreeAssets**: `bool` (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **CachePartOperationsAsync**(`partOperations: Array`) -> `null` [Yields]
- **CanEditAssetAsync**(`content: Content`) -> `bool` [Yields]
- **ComposeDecalAsync**(`decal: Decal`, `layers: Array`) -> `null` [Yields]
- **CreateAssetAsync**(`object: Object`, `assetType: AssetType`, `requestParameters: Dictionary = nil`) -> `Tuple` [Yields]
- **CreateAssetVersionAsync**(`object: Object`, `assetType: AssetType`, `assetId: int64`, `requestParameters: Dictionary = nil`) -> `Tuple` [Yields]
- **CreateDataModelContentAsync**(`content: Content`, `options: Dictionary?`) -> `Tuple` [Yields]
- **CreateEditableImage**(`editableImageOptions: Dictionary?`) -> `EditableImage`
- **CreateEditableImageAsync**(`content: Content`, `editableImageOptions: Dictionary?`) -> `EditableImage` [Yields]
- **CreateEditableMesh**(`editableMeshOptions: Dictionary?`) -> `EditableMesh`
- **CreateEditableMeshAsync**(`content: Content`, `editableMeshOptions: Dictionary?`) -> `EditableMesh` [Yields]
- **CreateMeshPartAsync**(`meshContent: Content`, `options: Dictionary = nil`) -> `MeshPart` [Yields]
- **CreatePlaceAsync**(`placeName: string`, `templatePlaceID: int64`, `description: string = `) -> `int64` [Yields]
- **CreatePlaceInPlayerInventoryAsync**(`player: Instance`, `placeName: string`, `templatePlaceID: int64`, `description: string = `) -> `int64` [Yields]
- **CreateSurfaceAppearanceAsync**(`content: Dictionary`) -> `SurfaceAppearance` [Yields]
- **DeserializeInstance**(`serializedInstance: string`) -> `Instance`
- **GetAssetIdsForPackage**(`packageAssetId: int64`) -> `Array` [Yields] [Deprecated]
- **GetAssetIdsForPackageAsync**(`packageAssetId: int64`) -> `Array` [Yields]
- **GetAudioMetadataAsync**(`idList: Array`) -> `Array` [Yields]
- **GetBundleDetailsAsync**(`bundleId: int64`) -> `Dictionary` [Yields]
- **GetCreatorAssetID**(`creationID: int64`) -> `int64` [Yields] [Deprecated]
- **GetGamePlacesAsync**() -> `Instance` [Yields]
- **GetOpaqueContentMetadataMap**(`opaqueContent: Content`) -> `Dictionary`
- **LoadAssetAsync**(`assetId: int64`) -> `Instance` [Yields]
- **PromptCreateAssetAsync**(`player: Player`, `instance: Instance`, `assetType: AssetType`) -> `Tuple` [Yields]
- **PromptImportAnimationClipFromVideoAsync**(`player: Player`, `progressCallback: Function`) -> `Tuple` [Yields]
- **SavePlaceAsync**(`requestParameters: Dictionary?`) -> `null` [Yields]
- **SearchAudio**(`searchParameters: AudioSearchParams`) -> `AudioPages` [Yields] [Deprecated]
- **SearchAudioAsync**(`searchParameters: AudioSearchParams`) -> `AudioPages` [Yields]

## Events

- **AudioMetadataFailedResponse**(`requestid: int64`)
- **AudioMetadataRequest**(`requestid: int64`, `request: Array`)
- **AudioMetadataResponse**(`requestid: int64`, `response: Array`)
- **OpenCreateResultModal**(`resultType: PromptCreateAssetResult`)
- **OpenPublishResultModal**(`resultType: PromptPublishAssetResult`)

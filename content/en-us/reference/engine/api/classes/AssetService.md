---
title: AssetService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# AssetService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.AssetService.AllowInsertFreeAssets` | `bool` |  {security: RobloxScriptSecurity} |

## Methods

### `Class.AssetService:CachePartOperationsAsync`

``CachePartOperationsAsync(partOperations: `Array`)`` → `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AssetService:CanEditAssetAsync`

``CanEditAssetAsync(content: `Datatype.Content`)`` → `bool`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AssetService:ComposeDecalAsync`

``ComposeDecalAsync(decal: `Class.Decal`, layers: `Array`)`` → `null`
  [Yields]

### `Class.AssetService:CreateAssetAsync`

``CreateAssetAsync(object: `Class.Object`, assetType: `Enum.AssetType`, requestParameters: `Dictionary`)`` → `Tuple`
  [Yields]

### `Class.AssetService:CreateAssetVersionAsync`

``CreateAssetVersionAsync(object: `Class.Object`, assetType: `Enum.AssetType`, assetId: `int64`, requestParameters: `Dictionary`)`` → `Tuple`
  [Yields]

### `Class.AssetService:CreateDataModelContentAsync`

``CreateDataModelContentAsync(content: `Datatype.Content`, options: `Dictionary?`)`` → `Tuple`
  [Yields]

### `Class.AssetService:CreateEditableImage`

``CreateEditableImage(editableImageOptions: `Dictionary?`)`` → `Class.EditableImage`

### `Class.AssetService:CreateEditableImageAsync`

``CreateEditableImageAsync(content: `Datatype.Content`, editableImageOptions: `Dictionary?`)`` → `Class.EditableImage`
  [Yields]

### `Class.AssetService:CreateEditableMesh`

``CreateEditableMesh(editableMeshOptions: `Dictionary?`)`` → `Class.EditableMesh`

### `Class.AssetService:CreateEditableMeshAsync`

``CreateEditableMeshAsync(content: `Datatype.Content`, editableMeshOptions: `Dictionary?`)`` → `Class.EditableMesh`
  [Yields]

### `Class.AssetService:CreateMeshPartAsync`

``CreateMeshPartAsync(meshContent: `Datatype.Content`, options: `Dictionary`)`` → `Class.MeshPart`
  [Yields]

### `Class.AssetService:CreatePlaceAsync`

``CreatePlaceAsync(placeName: `string`, templatePlaceID: `int64`, description: `string`)`` → `int64`
  [Yields]

### `Class.AssetService:CreatePlaceInPlayerInventoryAsync`

``CreatePlaceInPlayerInventoryAsync(player: `Class.Instance`, placeName: `string`, templatePlaceID: `int64`, description: `string`)`` → `int64`
  [Yields]

### `Class.AssetService:CreateSurfaceAppearanceAsync`

``CreateSurfaceAppearanceAsync(content: `Dictionary`)`` → `Class.SurfaceAppearance`
  [Yields]

### `Class.AssetService:DeserializeInstance`

``DeserializeInstance(serializedInstance: `string`)`` → `Class.Instance`
   {security: RobloxScriptSecurity}

### `Class.AssetService:GetAssetIdsForPackage`

``GetAssetIdsForPackage(packageAssetId: `int64`)`` → `Array`
  [Yields] [Deprecated]

### `Class.AssetService:GetAssetIdsForPackageAsync`

``GetAssetIdsForPackageAsync(packageAssetId: `int64`)`` → `Array`
  [Yields]

### `Class.AssetService:GetAudioMetadataAsync`

``GetAudioMetadataAsync(idList: `Array`)`` → `Array`
  [Yields]

### `Class.AssetService:GetBundleDetailsAsync`

``GetBundleDetailsAsync(bundleId: `int64`)`` → `Dictionary`
  [Yields]

### `Class.AssetService:GetCreatorAssetID`

``GetCreatorAssetID(creationID: `int64`)`` → `int64`
  [Yields] [Deprecated]

### `Class.AssetService:GetGamePlacesAsync`

``GetGamePlacesAsync()`` → `Class.Instance`
  [Yields]

### `Class.AssetService:GetOpaqueContentMetadataMap`

``GetOpaqueContentMetadataMap(opaqueContent: `Datatype.Content`)`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.AssetService:LoadAssetAsync`

``LoadAssetAsync(assetId: `int64`)`` → `Class.Instance`
  [Yields]

### `Class.AssetService:PromptCreateAssetAsync`

``PromptCreateAssetAsync(player: `Class.Player`, instance: `Class.Instance`, assetType: `Enum.AssetType`)`` → `Tuple`
  [Yields]

### `Class.AssetService:PromptImportAnimationClipFromVideoAsync`

``PromptImportAnimationClipFromVideoAsync(player: `Class.Player`, progressCallback: `Datatype.Function`)`` → `Tuple`
  [Yields]

### `Class.AssetService:SavePlaceAsync`

``SavePlaceAsync(requestParameters: `Dictionary?`)`` → `null`
  [Yields]

### `Class.AssetService:SearchAudio`

``SearchAudio(searchParameters: `Class.AudioSearchParams`)`` → `Class.AudioPages`
  [Yields] [Deprecated]

### `Class.AssetService:SearchAudioAsync`

``SearchAudioAsync(searchParameters: `Class.AudioSearchParams`)`` → `Class.AudioPages`
  [Yields]

## Events

### `Class.AssetService.AudioMetadataFailedResponse`

Fires with: (requestid: `int64`)

### `Class.AssetService.AudioMetadataRequest`

Fires with: (requestid: `int64`, request: `Array`)

### `Class.AssetService.AudioMetadataResponse`

Fires with: (requestid: `int64`, response: `Array`)

### `Class.AssetService.OpenCreateResultModal`

Fires with: (resultType: `Enum.PromptCreateAssetResult`)

### `Class.AssetService.OpenPublishResultModal`

Fires with: (resultType: `Enum.PromptPublishAssetResult`)

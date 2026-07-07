---
title: StudioAssetService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# StudioAssetService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **AutoSetupAvatarAsync**(`modelId: ContentId`, `progressCallback: Function`, `notificationCallback: Function?`, `options: Dictionary?`) -> `Instance` [Yields]
- **AutoSetupSerializedAvatarAsync**(`serializedInstance: string`, `publishInfo: Dictionary`, `telemetryMetadata: Dictionary`, `progressCallback: Function`, `notificationCallback: Function?`, `options: Dictionary?`) -> `Instance` [Yields]
- **CancelAutoSetupAvatarAsync**(`jobId: string`) -> `null` [Yields]
- **ConvertToPackageUpload**(`uploadUrl: string`, `cloneInstances: Instances`, `originalInstances: Instances`) -> `null`
- **DEPRECATED_SerializeInstances**(`instances: Instances`) -> `string` [Yields]
- **FireOnUGCSubmitCompleted**(`cancelled: bool`) -> `null`
- **PromptSaveInstanceToRobloxAsync**(`instance: Instance`, `assetType: Variant`, `groupId: int64?`) -> `Tuple` [Yields]
- **PublishPackage**(`instance: Instance`, `publishInfo: Dictionary`) -> `null`
- **RequestAvatarAutosetupAsync**(`meshId: ContentId`, `textureId: ContentId`, `progressCallback: Function`) -> `Instance` [Yields]
- **ResolveSaveInstanceToRoblox**(`requestId: string`, `assetId: int64?`, `assetName: string?`, `errorMessage: string?`) -> `null`
- **SerializeInstances**(`instances: Instances`, `groupId: int64 = 0`, `isPackage: bool = false`) -> `string` [Yields]
- **ShowSaveToRoblox**(`instances: Instances`, `assetType: Variant`, `hasSubsequent: bool = false`) -> `null`
- **UpdatePublishedPackage**(`assetmetadata: Dictionary`, `rootInstance: Instance`, `isConvert: bool = false`, `addUndoWaypoint: bool = false`) -> `null`

## Events

- **OnConvertToPackageResult**(`isSuccessful: bool`, `errorMessage: string`)
- **OnPromptSaveInstanceToRobloxAsync**(`instance: Instance`, `assetType: Variant`, `requestId: string`, `groupId: int64?`)
- **OnPublishPackageResult**(`result: Dictionary`, `errorMessage: string`)
- **OnSaveToRoblox**(`instances: Instances`, `assetType: Variant`, `hasSubsequent: bool`)
- **OnUGCSubmitCompleted**(`cancelled: bool`)

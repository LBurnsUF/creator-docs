---
title: StudioAssetService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# StudioAssetService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.StudioAssetService:AutoSetupAvatarAsync`

``AutoSetupAvatarAsync(modelId: `Datatype.ContentId`, progressCallback: `Datatype.Function`, notificationCallback: `Datatype.Function`?, options: `Dictionary?`)`` -> `Class.Instance`
  [Yields] {security: RobloxScriptSecurity}

### `Class.StudioAssetService:AutoSetupSerializedAvatarAsync`

``AutoSetupSerializedAvatarAsync(serializedInstance: `string`, publishInfo: `Dictionary`, telemetryMetadata: `Dictionary`, progressCallback: `Datatype.Function`, notificationCallback: `Datatype.Function`?, options: `Dictionary?`)`` -> `Class.Instance`
  [Yields] {security: RobloxScriptSecurity}

### `Class.StudioAssetService:CancelAutoSetupAvatarAsync`

``CancelAutoSetupAvatarAsync(jobId: `string`)`` -> `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.StudioAssetService:ConvertToPackageUpload`

``ConvertToPackageUpload(uploadUrl: `string`, cloneInstances: `Datatype.Instances`, originalInstances: `Datatype.Instances`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StudioAssetService:DEPRECATED_SerializeInstances`

``DEPRECATED_SerializeInstances(instances: `Datatype.Instances`)`` -> `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.StudioAssetService:FireOnUGCSubmitCompleted`

``FireOnUGCSubmitCompleted(cancelled: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StudioAssetService:PromptSaveInstanceToRobloxAsync`

``PromptSaveInstanceToRobloxAsync(instance: `Class.Instance`, assetType: `Variant`, groupId: `int64?`)`` -> `Tuple`
  [Yields] {security: RobloxScriptSecurity}

### `Class.StudioAssetService:PublishPackage`

``PublishPackage(instance: `Class.Instance`, publishInfo: `Dictionary`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StudioAssetService:RequestAvatarAutosetupAsync`

``RequestAvatarAutosetupAsync(meshId: `Datatype.ContentId`, textureId: `Datatype.ContentId`, progressCallback: `Datatype.Function`)`` -> `Class.Instance`
  [Yields] {security: RobloxScriptSecurity}

### `Class.StudioAssetService:ResolveSaveInstanceToRoblox`

``ResolveSaveInstanceToRoblox(requestId: `string`, assetId: `int64?`, assetName: `string?`, errorMessage: `string?`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StudioAssetService:SerializeInstances`

``SerializeInstances(instances: `Datatype.Instances`, groupId: `int64`, isPackage: `bool`)`` -> `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.StudioAssetService:ShowSaveToRoblox`

``ShowSaveToRoblox(instances: `Datatype.Instances`, assetType: `Variant`, hasSubsequent: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StudioAssetService:UpdatePublishedPackage`

``UpdatePublishedPackage(assetmetadata: `Dictionary`, rootInstance: `Class.Instance`, isConvert: `bool`, addUndoWaypoint: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.StudioAssetService.OnConvertToPackageResult`

Fires with: (isSuccessful: `bool`, errorMessage: `string`)

### `Class.StudioAssetService.OnPromptSaveInstanceToRobloxAsync`

Fires with: (instance: `Class.Instance`, assetType: `Variant`, requestId: `string`, groupId: `int64?`)

### `Class.StudioAssetService.OnPublishPackageResult`

Fires with: (result: `Dictionary`, errorMessage: `string`)

### `Class.StudioAssetService.OnSaveToRoblox`

Fires with: (instances: `Datatype.Instances`, assetType: `Variant`, hasSubsequent: `bool`)

### `Class.StudioAssetService.OnUGCSubmitCompleted`

Fires with: (cancelled: `bool`)

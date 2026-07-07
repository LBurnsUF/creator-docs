---
title: PublishService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# PublishService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.PublishService:CreateAssetAndWaitForAssetId`

``CreateAssetAndWaitForAssetId(instances: `Datatype.Instances`, operationId: `string`, creatorType: `Enum.AssetCreatorType`, creatorId: `int64`, assetType: `string`, name: `string`, description: `string`, expectedPrice: `int`)`` → `int64`
  [Yields] {security: RobloxScriptSecurity}

### `Class.PublishService:CreateAssetOrAssetVersionAndPollAssetWithTelemetryAsync`

``CreateAssetOrAssetVersionAndPollAssetWithTelemetryAsync(serializedInstance: `string`, creatorType: `Enum.AssetCreatorType`, creatorId: `int64`, assetType: `string`, assetId: `int64`, name: `string`, description: `string`, token: `string`, contentType: `string`, expectedPrice: `int`)`` → `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.PublishService:CreateAssetOrAssetVersionAndPollAssetWithTelemetryAsyncWithAddParam`

``CreateAssetOrAssetVersionAndPollAssetWithTelemetryAsyncWithAddParam(serializedInstance: `string`, publishInfo: `Dictionary`)`` → `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.PublishService:CreateAssetOrAssetVersionAndPollAssetWithTelemetryAsyncWithAddParamErrorJson`

``CreateAssetOrAssetVersionAndPollAssetWithTelemetryAsyncWithAddParamErrorJson(serializedInstance: `string`, publishInfo: `Dictionary`)`` → `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.PublishService:PublishCageMeshAsync`

``PublishCageMeshAsync(wrap: `Class.Instance`, cageType: `Enum.CageType`)`` → `Datatype.ContentId`
  [Yields] {security: RobloxScriptSecurity}

### `Class.PublishService:PublishDescendantAssets`

``PublishDescendantAssets(instance: `Class.Instance`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.PublishService:PublishDescendantAssetsAsync`

``PublishDescendantAssetsAsync(instance: `Class.Instance`)`` → `bool`
  [Yields] {security: RobloxScriptSecurity}

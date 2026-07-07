---
title: PublishService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# PublishService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **CreateAssetAndWaitForAssetId**(`instances: Instances`, `operationId: string`, `creatorType: AssetCreatorType`, `creatorId: int64`, `assetType: string`, `name: string`, `description: string`, `expectedPrice: int = 0`) -> `int64` [Yields]
- **CreateAssetOrAssetVersionAndPollAssetWithTelemetryAsync**(`serializedInstance: string`, `creatorType: AssetCreatorType`, `creatorId: int64`, `assetType: string`, `assetId: int64`, `name: string`, `description: string`, `token: string`, `contentType: string`, `expectedPrice: int = 0`) -> `Dictionary` [Yields]
- **CreateAssetOrAssetVersionAndPollAssetWithTelemetryAsyncWithAddParam**(`serializedInstance: string`, `publishInfo: Dictionary`) -> `Dictionary` [Yields]
- **CreateAssetOrAssetVersionAndPollAssetWithTelemetryAsyncWithAddParamErrorJson**(`serializedInstance: string`, `publishInfo: Dictionary`) -> `Dictionary` [Yields]
- **PublishCageMeshAsync**(`wrap: Instance`, `cageType: CageType`) -> `ContentId` [Yields]
- **PublishDescendantAssets**(`instance: Instance`) -> `bool`
- **PublishDescendantAssetsAsync**(`instance: Instance`) -> `bool` [Yields]

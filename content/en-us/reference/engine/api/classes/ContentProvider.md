---
title: ContentProvider
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ContentProvider

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **BaseUrl**: `string` [ReadOnly] [NotReplicated]
- **RequestQueueSize**: `int` [ReadOnly] [NotReplicated]

## Methods

- **GetAssetFetchStatus**(`contentId: ContentId`) -> `AssetFetchStatus`
- **GetAssetFetchStatusChangedSignal**(`contentId: ContentId`) -> `RBXScriptSignal`
- **GetDependencyContentIds**(`root: Instance`) -> `Array`
- **GetDetailedFailedRequests**() -> `Array`
- **GetFailedRequests**() -> `Array`
- **ListEncryptedAssets**() -> `Array`
- **Preload**(`contentId: ContentId`) -> `null` [Deprecated]
- **PreloadAsync**(`contentIdList: Array`, `callbackFunction: Function = nil`) -> `null` [Yields]
- **RegisterDefaultEncryptionKey**(`encryptionKey: string`) -> `null`
- **RegisterDefaultSessionKey**(`sessionKey: string`) -> `null`
- **RegisterEncryptedAsset**(`assetId: ContentId`, `encryptionKey: string`) -> `null`
- **RegisterSessionEncryptedAsset**(`contentId: ContentId`, `sessionKey: string`) -> `null`
- **SetBaseUrl**(`url: string`) -> `null`
- **UnregisterDefaultEncryptionKey**() -> `null`
- **UnregisterEncryptedAsset**(`assetId: ContentId`) -> `null`

## Events

- **AssetFetchFailed**(`assetId: ContentId`)

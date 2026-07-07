---
title: ContentProvider
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ContentProvider

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.ContentProvider.BaseUrl` | `string` | [ReadOnly] [NotReplicated] |
| `Class.ContentProvider.RequestQueueSize` | `int` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.ContentProvider:GetAssetFetchStatus`

``GetAssetFetchStatus(contentId: `Datatype.ContentId`)`` → `Enum.AssetFetchStatus`

### `Class.ContentProvider:GetAssetFetchStatusChangedSignal`

``GetAssetFetchStatusChangedSignal(contentId: `Datatype.ContentId`)`` → `Datatype.RBXScriptSignal`

### `Class.ContentProvider:GetDependencyContentIds`

``GetDependencyContentIds(root: `Class.Instance`)`` → `Array`
   {security: RobloxScriptSecurity}

### `Class.ContentProvider:GetDetailedFailedRequests`

``GetDetailedFailedRequests()`` → `Array`
   {security: RobloxScriptSecurity}

### `Class.ContentProvider:GetFailedRequests`

``GetFailedRequests()`` → `Array`
   {security: RobloxScriptSecurity}

### `Class.ContentProvider:ListEncryptedAssets`

``ListEncryptedAssets()`` → `Array`

### `Class.ContentProvider:Preload`

``Preload(contentId: `Datatype.ContentId`)`` → `null`
  [Deprecated]

### `Class.ContentProvider:PreloadAsync`

``PreloadAsync(contentIdList: `Array`, callbackFunction: `Datatype.Function`)`` → `null`
  [Yields]

### `Class.ContentProvider:RegisterDefaultEncryptionKey`

``RegisterDefaultEncryptionKey(encryptionKey: `string`)`` → `null`

### `Class.ContentProvider:RegisterDefaultSessionKey`

``RegisterDefaultSessionKey(sessionKey: `string`)`` → `null`

### `Class.ContentProvider:RegisterEncryptedAsset`

``RegisterEncryptedAsset(assetId: `Datatype.ContentId`, encryptionKey: `string`)`` → `null`

### `Class.ContentProvider:RegisterSessionEncryptedAsset`

``RegisterSessionEncryptedAsset(contentId: `Datatype.ContentId`, sessionKey: `string`)`` → `null`

### `Class.ContentProvider:SetBaseUrl`

``SetBaseUrl(url: `string`)`` → `null`
   {security: LocalUserSecurity}

### `Class.ContentProvider:UnregisterDefaultEncryptionKey`

``UnregisterDefaultEncryptionKey()`` → `null`

### `Class.ContentProvider:UnregisterEncryptedAsset`

``UnregisterEncryptedAsset(assetId: `Datatype.ContentId`)`` → `null`

## Events

### `Class.ContentProvider.AssetFetchFailed`

Fires with: (assetId: `Datatype.ContentId`)

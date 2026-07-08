---
title: ContentProvider
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ContentProvider

Service that is used to load content, or assets, into a game.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

Service that loads content (assets) into a game.

Roblox servers stream all assets to the client at runtime: objects in the
Workspace, mesh assets, texture assets, etc. Assets such as mesh visual data,
textures, decals, and sounds are streamed in as required, regardless of
whether [Streaming](../../../workspace/streaming/index.md) is enabled.

In some cases, this behavior is undesirable, as it can lead to a delay before
the content loads into the experience.

`ContentProvider` lets you preload assets into an experience using the
`Class.ContentProvider:PreloadAsync()` method. You might want to display a
loading screen, preload critical assets, and only then allow the player into
the experience.

#### Best Practices for Preloading

- Only preload essential assets, **not** the entire `Class.Workspace`. You
  might get occasional pop-in, but it decreases load times and generally
  doesn't disrupt the player experience. Assets that are good candidates for
  preloading include those required for the loading screen, the UI, or the
  starting area.
- Let players skip the loading screen, or automatically skip it after a
  certain amount of time.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ContentProvider.BaseUrl` | `string` | [ReadOnly] [NotReplicated] |
| `Class.ContentProvider.RequestQueueSize` | `int` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.ContentProvider:GetAssetFetchStatus`

``GetAssetFetchStatus(contentId: `Datatype.ContentId`)`` -> `Enum.AssetFetchStatus`

### `Class.ContentProvider:GetAssetFetchStatusChangedSignal`

``GetAssetFetchStatusChangedSignal(contentId: `Datatype.ContentId`)`` -> `Datatype.RBXScriptSignal`

### `Class.ContentProvider:GetDependencyContentIds`

``GetDependencyContentIds(root: `Class.Instance`)`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.ContentProvider:GetDetailedFailedRequests`

``GetDetailedFailedRequests()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.ContentProvider:GetFailedRequests`

``GetFailedRequests()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.ContentProvider:ListEncryptedAssets`

``ListEncryptedAssets()`` -> `Array`

### `Class.ContentProvider:Preload`

``Preload(contentId: `Datatype.ContentId`)`` -> `null`
  [Deprecated]

### `Class.ContentProvider:PreloadAsync`

``PreloadAsync(contentIdList: `Array`, callbackFunction: `Datatype.Function`)`` -> `null`
  [Yields]

### `Class.ContentProvider:RegisterDefaultEncryptionKey`

``RegisterDefaultEncryptionKey(encryptionKey: `string`)`` -> `null`

### `Class.ContentProvider:RegisterDefaultSessionKey`

``RegisterDefaultSessionKey(sessionKey: `string`)`` -> `null`

### `Class.ContentProvider:RegisterEncryptedAsset`

``RegisterEncryptedAsset(assetId: `Datatype.ContentId`, encryptionKey: `string`)`` -> `null`

### `Class.ContentProvider:RegisterSessionEncryptedAsset`

``RegisterSessionEncryptedAsset(contentId: `Datatype.ContentId`, sessionKey: `string`)`` -> `null`

### `Class.ContentProvider:SetBaseUrl`

``SetBaseUrl(url: `string`)`` -> `null`
   {security: LocalUserSecurity}

### `Class.ContentProvider:UnregisterDefaultEncryptionKey`

``UnregisterDefaultEncryptionKey()`` -> `null`

### `Class.ContentProvider:UnregisterEncryptedAsset`

``UnregisterEncryptedAsset(assetId: `Datatype.ContentId`)`` -> `null`

## Events

### `Class.ContentProvider.AssetFetchFailed`

Fires with: (assetId: `Datatype.ContentId`)

---
title: InsertService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# InsertService

Used to insert assets from the Roblox website.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

InsertService is used to insert assets from the Roblox website, typically the
`Class.InsertService:LoadAsset()|LoadAsset` function.

To load an asset, it must be accessible by the creator of the experience
loading it, which can be either a user or group. Should an experience be
uploaded by a different creator, the asset data would not be accessible. See
the `Class.InsertService:LoadAsset()|LoadAsset()` method for more details on
this security check. Note that you should **not** use this service for loading
API keys or other secrets. Use `Class.HttpService:GetSecret()` instead.

#### See Also

- `Class.AssetService`, which can provide information about assets you might
  want to load using InsertService

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.InsertService.AllowInsertFreeModels` | `bool` | [NotReplicated] [NotBrowsable] [Deprecated] |

## Methods

### `Class.InsertService:ApproveAssetId`

``ApproveAssetId(assetId: `int64`)`` -> `null`
  [Deprecated]

### `Class.InsertService:ApproveAssetVersionId`

``ApproveAssetVersionId(assetVersionId: `int64`)`` -> `null`
  [Deprecated]

### `Class.InsertService:CreateMeshPartAsync`

``CreateMeshPartAsync(meshId: `Datatype.ContentId`, collisionFidelity: `Enum.CollisionFidelity`, renderFidelity: `Enum.RenderFidelity`)`` -> `Class.MeshPart`
  [Yields]

### `Class.InsertService:GetBaseCategories`

``GetBaseCategories()`` -> `Array`
  [Yields] [Deprecated]

### `Class.InsertService:GetBaseSets`

``GetBaseSets()`` -> `Array`
  [Yields] [Deprecated]

### `Class.InsertService:GetCollection`

``GetCollection(categoryId: `int64`)`` -> `Array`
  [Yields] [Deprecated]

### `Class.InsertService:GetFreeDecals`

``GetFreeDecals(searchText: `string`, pageNum: `int`)`` -> `Array`
  [Yields] [Deprecated]

### `Class.InsertService:GetFreeDecalsAsync`

``GetFreeDecalsAsync(searchText: `string`, pageNum: `int`)`` -> `Array`
  [Yields]

### `Class.InsertService:GetFreeModels`

``GetFreeModels(searchText: `string`, pageNum: `int`)`` -> `Array`
  [Yields] [Deprecated]

### `Class.InsertService:GetFreeModelsAsync`

``GetFreeModelsAsync(searchText: `string`, pageNum: `int`)`` -> `Array`
  [Yields]

### `Class.InsertService:GetLatestAssetVersionAsync`

``GetLatestAssetVersionAsync(assetId: `int64`)`` -> `int64`
  [Yields]

### `Class.InsertService:GetLocalFileContents`

``GetLocalFileContents(contentId: `string`)`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.InsertService:GetUserCategories`

``GetUserCategories(userId: `Datatype.User`)`` -> `Array`
  [Yields] [Deprecated]

### `Class.InsertService:GetUserSets`

``GetUserSets(userId: `Datatype.User`)`` -> `Array`
  [Yields] [Deprecated]

### `Class.InsertService:Insert`

``Insert(instance: `Class.Instance`)`` -> `null`
  [Deprecated]

### `Class.InsertService:LoadAsset`

``LoadAsset(assetId: `int64`)`` -> `Class.Instance`
  [Yields]

### `Class.InsertService:LoadAssetVersion`

``LoadAssetVersion(assetVersionId: `int64`)`` -> `Class.Instance`
  [Yields]

### `Class.InsertService:LoadAssetWithBytecodeAsync`

``LoadAssetWithBytecodeAsync(assetId: `int64`, version: `int64`)`` -> `Class.Instance`
  [Yields] {security: RobloxScriptSecurity}

### `Class.InsertService:LoadAssetWithFormat`

``LoadAssetWithFormat(assetId: `int64`, format: `string`)`` -> `Datatype.Instances`
  [Yields] {security: RobloxScriptSecurity}

### `Class.InsertService:LoadLocalAsset`

``LoadLocalAsset(assetPath: `string`)`` -> `Class.Instance`
   {security: RobloxScriptSecurity}

### `Class.InsertService:LoadPackageAssetAsync`

``LoadPackageAssetAsync(url: `Datatype.ContentId`)`` -> `Datatype.Instances`
  [Yields] {security: RobloxScriptSecurity}

### `Class.InsertService:loadAsset`

``loadAsset(assetId: `int64`)`` -> `Class.Instance`
  [Yields] [Deprecated]

---
title: InsertService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# InsertService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.InsertService.AllowInsertFreeModels` | `bool` | [NotReplicated] [NotBrowsable] [Deprecated] |

## Methods

### `Class.InsertService:ApproveAssetId`

``ApproveAssetId(assetId: `int64`)`` → `null`
  [Deprecated]

### `Class.InsertService:ApproveAssetVersionId`

``ApproveAssetVersionId(assetVersionId: `int64`)`` → `null`
  [Deprecated]

### `Class.InsertService:CreateMeshPartAsync`

``CreateMeshPartAsync(meshId: `Datatype.ContentId`, collisionFidelity: `Enum.CollisionFidelity`, renderFidelity: `Enum.RenderFidelity`)`` → `Class.MeshPart`
  [Yields]

### `Class.InsertService:GetBaseCategories`

``GetBaseCategories()`` → `Array`
  [Yields] [Deprecated]

### `Class.InsertService:GetBaseSets`

``GetBaseSets()`` → `Array`
  [Yields] [Deprecated]

### `Class.InsertService:GetCollection`

``GetCollection(categoryId: `int64`)`` → `Array`
  [Yields] [Deprecated]

### `Class.InsertService:GetFreeDecals`

``GetFreeDecals(searchText: `string`, pageNum: `int`)`` → `Array`
  [Yields] [Deprecated]

### `Class.InsertService:GetFreeDecalsAsync`

``GetFreeDecalsAsync(searchText: `string`, pageNum: `int`)`` → `Array`
  [Yields]

### `Class.InsertService:GetFreeModels`

``GetFreeModels(searchText: `string`, pageNum: `int`)`` → `Array`
  [Yields] [Deprecated]

### `Class.InsertService:GetFreeModelsAsync`

``GetFreeModelsAsync(searchText: `string`, pageNum: `int`)`` → `Array`
  [Yields]

### `Class.InsertService:GetLatestAssetVersionAsync`

``GetLatestAssetVersionAsync(assetId: `int64`)`` → `int64`
  [Yields]

### `Class.InsertService:GetLocalFileContents`

``GetLocalFileContents(contentId: `string`)`` → `string`
   {security: RobloxScriptSecurity}

### `Class.InsertService:GetUserCategories`

``GetUserCategories(userId: `Datatype.User`)`` → `Array`
  [Yields] [Deprecated]

### `Class.InsertService:GetUserSets`

``GetUserSets(userId: `Datatype.User`)`` → `Array`
  [Yields] [Deprecated]

### `Class.InsertService:Insert`

``Insert(instance: `Class.Instance`)`` → `null`
  [Deprecated]

### `Class.InsertService:LoadAsset`

``LoadAsset(assetId: `int64`)`` → `Class.Instance`
  [Yields]

### `Class.InsertService:LoadAssetVersion`

``LoadAssetVersion(assetVersionId: `int64`)`` → `Class.Instance`
  [Yields]

### `Class.InsertService:LoadAssetWithBytecodeAsync`

``LoadAssetWithBytecodeAsync(assetId: `int64`, version: `int64`)`` → `Class.Instance`
  [Yields] {security: RobloxScriptSecurity}

### `Class.InsertService:LoadAssetWithFormat`

``LoadAssetWithFormat(assetId: `int64`, format: `string`)`` → `Datatype.Instances`
  [Yields] {security: RobloxScriptSecurity}

### `Class.InsertService:LoadLocalAsset`

``LoadLocalAsset(assetPath: `string`)`` → `Class.Instance`
   {security: RobloxScriptSecurity}

### `Class.InsertService:LoadPackageAssetAsync`

``LoadPackageAssetAsync(url: `Datatype.ContentId`)`` → `Datatype.Instances`
  [Yields] {security: RobloxScriptSecurity}

### `Class.InsertService:loadAsset`

``loadAsset(assetId: `int64`)`` → `Class.Instance`
  [Yields] [Deprecated]

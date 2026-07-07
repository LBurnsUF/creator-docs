---
title: InsertService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# InsertService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **AllowInsertFreeModels**: `bool` [NotReplicated] [NotBrowsable] [Deprecated]

## Methods

- **ApproveAssetId**(`assetId: int64`) -> `null` [Deprecated]
- **ApproveAssetVersionId**(`assetVersionId: int64`) -> `null` [Deprecated]
- **CreateMeshPartAsync**(`meshId: ContentId`, `collisionFidelity: CollisionFidelity`, `renderFidelity: RenderFidelity`) -> `MeshPart` [Yields]
- **GetBaseCategories**() -> `Array` [Yields] [Deprecated]
- **GetBaseSets**() -> `Array` [Yields] [Deprecated]
- **GetCollection**(`categoryId: int64`) -> `Array` [Yields] [Deprecated]
- **GetFreeDecals**(`searchText: string`, `pageNum: int`) -> `Array` [Yields] [Deprecated]
- **GetFreeDecalsAsync**(`searchText: string`, `pageNum: int`) -> `Array` [Yields]
- **GetFreeModels**(`searchText: string`, `pageNum: int`) -> `Array` [Yields] [Deprecated]
- **GetFreeModelsAsync**(`searchText: string`, `pageNum: int`) -> `Array` [Yields]
- **GetLatestAssetVersionAsync**(`assetId: int64`) -> `int64` [Yields]
- **GetLocalFileContents**(`contentId: string`) -> `string`
- **GetUserCategories**(`userId: User`) -> `Array` [Yields] [Deprecated]
- **GetUserSets**(`userId: User`) -> `Array` [Yields] [Deprecated]
- **Insert**(`instance: Instance`) -> `null` [Deprecated]
- **LoadAsset**(`assetId: int64`) -> `Instance` [Yields]
- **LoadAssetVersion**(`assetVersionId: int64`) -> `Instance` [Yields]
- **LoadAssetWithBytecodeAsync**(`assetId: int64`, `version: int64`) -> `Instance` [Yields]
- **LoadAssetWithFormat**(`assetId: int64`, `format: string`) -> `Instances` [Yields]
- **LoadLocalAsset**(`assetPath: string`) -> `Instance`
- **LoadPackageAssetAsync**(`url: ContentId`) -> `Instances` [Yields]
- **loadAsset**(`assetId: int64`) -> `Instance` [Yields] [Deprecated]

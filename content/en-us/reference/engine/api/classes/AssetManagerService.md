---
title: AssetManagerService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# AssetManagerService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **AddNewPlace**() -> `int64` [Yields]
- **CreateAlias**(`assetType: int`, `assetId: int64`, `aliasName: string`) -> `null` [Yields]
- **DeleteAlias**(`aliasName: string`) -> `null` [Yields]
- **GetMeshIdFromAliasName**(`aliasName: string`) -> `int64`
- **GetMeshIdFromAssetId**(`assetId: int64`) -> `int64`
- **GetTextureIdFromAliasName**(`aliasName: string`) -> `int64`
- **GetTextureIdFromAssetId**(`assetId: int64`) -> `int64`
- **InsertAudio**(`assetId: int64`, `assetName: string`) -> `null`
- **InsertImage**(`assetId: int64`) -> `null`
- **InsertImages**(`assetIds: Array`) -> `null`
- **InsertMesh**(`aliasName: string`, `insertWithLocation: bool`, `sourceAssetId: int64`) -> `null`
- **InsertMeshesWithLocation**(`aliasNames: Array`, `meshIds: Array`) -> `null`
- **InsertModel**(`modelId: int64`) -> `null`
- **InsertPackage**(`packageId: int64`) -> `null`
- **InsertVideo**(`assetId: int64`, `assetName: string`) -> `null`
- **OpenPlace**(`placeId: int64`) -> `null`
- **RemovePlace**(`placeId: int64`) -> `null` [Yields]
- **RenameAlias**(`assetType: int`, `assetId: int64`, `oldAliasName: string`, `newAliasName: string`) -> `null` [Yields]
- **RenameModel**(`modelId: int64`, `newName: string`) -> `null` [Yields]
- **RenamePlace**(`placeId: int64`, `newName: string`) -> `null` [Yields]
- **ShowPackageDetails**(`packageId: int64`) -> `null`
- **UpdateAllPackages**(`packageId: int64`) -> `null`
- **ViewPackageOnWebsite**(`packageId: int64`) -> `null`

## Events

- **AssetImportedSignal**(`assetType: AssetType`, `assetId: string`, `assetName: int64`)
- **ImportSessionFinished**()
- **ImportSessionStarted**()

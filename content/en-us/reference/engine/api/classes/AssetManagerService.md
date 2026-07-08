---
title: AssetManagerService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# AssetManagerService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.AssetManagerService:AddNewPlace`

``AddNewPlace()`` -> `int64`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AssetManagerService:CreateAlias`

``CreateAlias(assetType: `int`, assetId: `int64`, aliasName: `string`)`` -> `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AssetManagerService:DeleteAlias`

``DeleteAlias(aliasName: `string`)`` -> `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AssetManagerService:GetMeshIdFromAliasName`

``GetMeshIdFromAliasName(aliasName: `string`)`` -> `int64`
   {security: RobloxScriptSecurity}

### `Class.AssetManagerService:GetMeshIdFromAssetId`

``GetMeshIdFromAssetId(assetId: `int64`)`` -> `int64`
   {security: RobloxScriptSecurity}

### `Class.AssetManagerService:GetTextureIdFromAliasName`

``GetTextureIdFromAliasName(aliasName: `string`)`` -> `int64`
   {security: RobloxScriptSecurity}

### `Class.AssetManagerService:GetTextureIdFromAssetId`

``GetTextureIdFromAssetId(assetId: `int64`)`` -> `int64`
   {security: RobloxScriptSecurity}

### `Class.AssetManagerService:InsertAudio`

``InsertAudio(assetId: `int64`, assetName: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AssetManagerService:InsertImage`

``InsertImage(assetId: `int64`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AssetManagerService:InsertImages`

``InsertImages(assetIds: `Array`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AssetManagerService:InsertMesh`

``InsertMesh(aliasName: `string`, insertWithLocation: `bool`, sourceAssetId: `int64`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AssetManagerService:InsertMeshesWithLocation`

``InsertMeshesWithLocation(aliasNames: `Array`, meshIds: `Array`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AssetManagerService:InsertModel`

``InsertModel(modelId: `int64`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AssetManagerService:InsertPackage`

``InsertPackage(packageId: `int64`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AssetManagerService:InsertVideo`

``InsertVideo(assetId: `int64`, assetName: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AssetManagerService:OpenPlace`

``OpenPlace(placeId: `int64`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AssetManagerService:RemovePlace`

``RemovePlace(placeId: `int64`)`` -> `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AssetManagerService:RenameAlias`

``RenameAlias(assetType: `int`, assetId: `int64`, oldAliasName: `string`, newAliasName: `string`)`` -> `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AssetManagerService:RenameModel`

``RenameModel(modelId: `int64`, newName: `string`)`` -> `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AssetManagerService:RenamePlace`

``RenamePlace(placeId: `int64`, newName: `string`)`` -> `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AssetManagerService:ShowPackageDetails`

``ShowPackageDetails(packageId: `int64`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AssetManagerService:UpdateAllPackages`

``UpdateAllPackages(packageId: `int64`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AssetManagerService:ViewPackageOnWebsite`

``ViewPackageOnWebsite(packageId: `int64`)`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.AssetManagerService.AssetImportedSignal`

Fires with: (assetType: `Enum.AssetType`, assetId: `string`, assetName: `int64`)

### `Class.AssetManagerService.ImportSessionFinished`

Fires with: ()

### `Class.AssetManagerService.ImportSessionStarted`

Fires with: ()

---
title: AvatarEditorService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# AvatarEditorService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.AvatarEditorService:BustAvatarFetchCache`

``BustAvatarFetchCache()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:CheckApplyDefaultClothing`

``CheckApplyDefaultClothing(humanoidDescription: `Class.HumanoidDescription`)`` → `Class.HumanoidDescription`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:CheckApplyDefaultClothingAsync`

``CheckApplyDefaultClothingAsync(humanoidDescription: `Class.HumanoidDescription`)`` → `Class.HumanoidDescription`
  [Yields]

### `Class.AvatarEditorService:ConformToAvatarRules`

``ConformToAvatarRules(humanoidDescription: `Class.HumanoidDescription`)`` → `Class.HumanoidDescription`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:ConformToAvatarRulesAsync`

``ConformToAvatarRulesAsync(humanoidDescription: `Class.HumanoidDescription`)`` → `Class.HumanoidDescription`
  [Yields]

### `Class.AvatarEditorService:GetAccessoryType`

``GetAccessoryType(avatarAssetType: `Enum.AvatarAssetType`)`` → `Enum.AccessoryType`

### `Class.AvatarEditorService:GetAvatarRules`

``GetAvatarRules()`` → `Dictionary`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:GetAvatarRulesAsync`

``GetAvatarRulesAsync()`` → `Dictionary`
  [Yields]

### `Class.AvatarEditorService:GetBatchItemDetails`

``GetBatchItemDetails(itemIds: `Array`, itemType: `Enum.AvatarItemType`)`` → `Array`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:GetBatchItemDetailsAsync`

``GetBatchItemDetailsAsync(itemIds: `Array`, itemType: `Enum.AvatarItemType`)`` → `Array`
  [Yields]

### `Class.AvatarEditorService:GetBundlesByAssetIdAsync`

``GetBundlesByAssetIdAsync(assetId: `int64`, limit: `int64`)`` → `Class.CatalogPages`
  [Yields]

### `Class.AvatarEditorService:GetFavorite`

``GetFavorite(itemId: `int64`, itemType: `Enum.AvatarItemType`)`` → `bool`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:GetFavoriteAsync`

``GetFavoriteAsync(itemId: `int64`, itemType: `Enum.AvatarItemType`)`` → `bool`
  [Yields]

### `Class.AvatarEditorService:GetHeadShapesAsync`

``GetHeadShapesAsync()`` → `Array`
  [Yields]

### `Class.AvatarEditorService:GetInventory`

``GetInventory(assetTypes: `Array`)`` → `Class.InventoryPages`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:GetInventoryAsync`

``GetInventoryAsync(assetTypes: `Array`)`` → `Class.InventoryPages`
  [Yields]

### `Class.AvatarEditorService:GetItemDetails`

``GetItemDetails(itemId: `int64`, itemType: `Enum.AvatarItemType`)`` → `Dictionary`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:GetItemDetailsAsync`

``GetItemDetailsAsync(itemId: `int64`, itemType: `Enum.AvatarItemType`)`` → `Dictionary`
  [Yields]

### `Class.AvatarEditorService:GetOutfitDetails`

``GetOutfitDetails(outfitId: `int64`)`` → `Dictionary`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:GetOutfitDetailsAsync`

``GetOutfitDetailsAsync(outfitId: `int64`)`` → `Dictionary`
  [Yields]

### `Class.AvatarEditorService:GetOutfits`

``GetOutfits(outfitSource: `Enum.OutfitSource`, outfitType: `Enum.OutfitType`)`` → `Class.OutfitPages`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:GetOutfitsAsync`

``GetOutfitsAsync(outfitSource: `Enum.OutfitSource`, outfitType: `Enum.OutfitType`)`` → `Class.OutfitPages`
  [Yields]

### `Class.AvatarEditorService:GetRecommendedAssets`

``GetRecommendedAssets(assetType: `Enum.AvatarAssetType`, contextAssetId: `int64`)`` → `Array`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:GetRecommendedAssetsAsync`

``GetRecommendedAssetsAsync(assetType: `Enum.AvatarAssetType`, contextAssetId: `int64`)`` → `Array`
  [Yields]

### `Class.AvatarEditorService:GetRecommendedBundles`

``GetRecommendedBundles(bundleId: `int64`)`` → `Array`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:GetRecommendedBundlesAsync`

``GetRecommendedBundlesAsync(bundleId: `int64`)`` → `Array`
  [Yields]

### `Class.AvatarEditorService:NoPromptApplyProfileConfiguration`

``NoPromptApplyProfileConfiguration(profileConfiguration: `Dictionary`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:NoPromptCreateOutfit`

``NoPromptCreateOutfit(humanoidDescription: `Class.HumanoidDescription`, rigType: `Enum.HumanoidRigType`, name: `string`, gearAssetId: `int64`, outfitOptions: `Dictionary`, outfitType: `Variant`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:NoPromptDeleteOutfit`

``NoPromptDeleteOutfit(outfitId: `int64`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:NoPromptRenameOutfit`

``NoPromptRenameOutfit(outfitId: `int64`, name: `string`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:NoPromptSaveAvatar`

``NoPromptSaveAvatar(humanoidDescription: `Class.HumanoidDescription`, rigType: `Enum.HumanoidRigType`, saveDict: `Dictionary`, gearAssetId: `int64`, profileConfiguration: `Dictionary`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:NoPromptSaveAvatarThumbnailCustomization`

``NoPromptSaveAvatarThumbnailCustomization(thumbnailType: `Enum.AvatarThumbnailCustomizationType`, emoteAssetId: `int64`, cameraDistanceScale: `float`, yRotDeg: `float`, fieldOfViewDeg: `float`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:NoPromptSetFavorite`

``NoPromptSetFavorite(itemId: `int64`, itemType: `Enum.AvatarItemType`, shouldFavorite: `bool`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:NoPromptUpdateOutfit`

``NoPromptUpdateOutfit(outfitId: `int64`, humanoidDescription: `Class.HumanoidDescription`, rigType: `Enum.HumanoidRigType`, gearAssetId: `int64`, outfitOptions: `Dictionary`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:PerformCreateOutfitWithDescription`

``PerformCreateOutfitWithDescription(humanoidDescription: `Class.HumanoidDescription`, name: `string`, profileConfiguration: `Dictionary`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:PerformDeleteOutfit`

``PerformDeleteOutfit()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:PerformRenameOutfit`

``PerformRenameOutfit(name: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:PerformSaveAvatarWithDescription`

``PerformSaveAvatarWithDescription(humanoidDescription: `Class.HumanoidDescription`, addedAssets: `Array`, removedAssets: `Array`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:PerformSetFavorite`

``PerformSetFavorite()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:PerformUpdateOutfit`

``PerformUpdateOutfit(humanoidDescription: `Class.HumanoidDescription`, profileConfiguration: `Dictionary`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:PromptAllowInventoryReadAccess`

``PromptAllowInventoryReadAccess()`` → `null`

### `Class.AvatarEditorService:PromptCreateOutfit`

``PromptCreateOutfit(outfit: `Class.HumanoidDescription`, rigType: `Enum.HumanoidRigType`, outfitOptions: `Dictionary`, outfitType: `Variant`)`` → `null`

### `Class.AvatarEditorService:PromptDeleteOutfit`

``PromptDeleteOutfit(outfitId: `int64`)`` → `null`

### `Class.AvatarEditorService:PromptRenameOutfit`

``PromptRenameOutfit(outfitId: `int64`)`` → `null`

### `Class.AvatarEditorService:PromptSaveAvatar`

``PromptSaveAvatar(humanoidDescription: `Class.HumanoidDescription`, rigType: `Enum.HumanoidRigType`)`` → `null`

### `Class.AvatarEditorService:PromptSetFavorite`

``PromptSetFavorite(itemId: `int64`, itemType: `Enum.AvatarItemType`, shouldFavorite: `bool`)`` → `null`

### `Class.AvatarEditorService:PromptUpdateOutfit`

``PromptUpdateOutfit(outfitId: `int64`, updatedOutfit: `Class.HumanoidDescription`, rigType: `Enum.HumanoidRigType`)`` → `null`

### `Class.AvatarEditorService:SearchCatalog`

``SearchCatalog(searchParameters: `Datatype.CatalogSearchParams`)`` → `Class.CatalogPages`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:SearchCatalogAsync`

``SearchCatalogAsync(searchParameters: `Datatype.CatalogSearchParams`)`` → `Class.CatalogPages`
  [Yields]

### `Class.AvatarEditorService:SetAllowInventoryReadAccess`

``SetAllowInventoryReadAccess(inventoryReadAccessGranted: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalCreateOutfitFailed`

``SignalCreateOutfitFailed()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalCreateOutfitPermissionDenied`

``SignalCreateOutfitPermissionDenied()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalDeleteOutfitFailed`

``SignalDeleteOutfitFailed()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalDeleteOutfitPermissionDenied`

``SignalDeleteOutfitPermissionDenied()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalRenameOutfitFailed`

``SignalRenameOutfitFailed()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalRenameOutfitPermissionDenied`

``SignalRenameOutfitPermissionDenied()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalSaveAvatarFailed`

``SignalSaveAvatarFailed()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalSaveAvatarPermissionDenied`

``SignalSaveAvatarPermissionDenied()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalSetFavoriteFailed`

``SignalSetFavoriteFailed()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalSetFavoritePermissionDenied`

``SignalSetFavoritePermissionDenied()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalUpdateOutfitFailed`

``SignalUpdateOutfitFailed()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalUpdateOutfitPermissionDenied`

``SignalUpdateOutfitPermissionDenied()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:refreshAvatarThumbnails`

``refreshAvatarThumbnails(thumbnailTypes: `Array`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.AvatarEditorService.OpenAllowInventoryReadAccess`

Fires with: ()

### `Class.AvatarEditorService.OpenPromptCreateOufit`

Fires with: (humanoidDescription: `Class.HumanoidDescription`, rigType: `Enum.HumanoidRigType`)

### `Class.AvatarEditorService.OpenPromptDeleteOutfit`

Fires with: (outfitId: `int64`)

### `Class.AvatarEditorService.OpenPromptRenameOutfit`

Fires with: (outfitId: `int64`)

### `Class.AvatarEditorService.OpenPromptSaveAvatar`

Fires with: (humanoidDescription: `Class.HumanoidDescription`, rigType: `Enum.HumanoidRigType`)

### `Class.AvatarEditorService.OpenPromptSetFavorite`

Fires with: (itemId: `int64`, itemType: `Enum.AvatarItemType`, shouldFavorite: `bool`)

### `Class.AvatarEditorService.OpenPromptUpdateOutfit`

Fires with: (outfitId: `int64`, humanoidDescription: `Class.HumanoidDescription`, rigType: `Enum.HumanoidRigType`)

### `Class.AvatarEditorService.PromptAllowInventoryReadAccessCompleted`

Fires with: (result: `Enum.AvatarPromptResult`)

### `Class.AvatarEditorService.PromptApplyProfileConfigurationCompleted`

Fires with: (result: `Enum.AvatarPromptResult`)

### `Class.AvatarEditorService.PromptCreateOutfitCompleted`

Fires with: (result: `Enum.AvatarPromptResult`, failureType: `Variant`)

### `Class.AvatarEditorService.PromptDeleteOutfitCompleted`

Fires with: (result: `Enum.AvatarPromptResult`)

### `Class.AvatarEditorService.PromptRenameOutfitCompleted`

Fires with: (result: `Enum.AvatarPromptResult`)

### `Class.AvatarEditorService.PromptSaveAvatarCompleted`

Fires with: (result: `Enum.AvatarPromptResult`, humanoidDescription: `Class.HumanoidDescription`)

### `Class.AvatarEditorService.PromptSaveAvatarThumbnailCustomizationCompleted`

Fires with: (result: `Enum.AvatarPromptResult`, failureType: `Variant`)

### `Class.AvatarEditorService.PromptSetFavoriteCompleted`

Fires with: (result: `Enum.AvatarPromptResult`)

### `Class.AvatarEditorService.PromptUpdateOutfitCompleted`

Fires with: (result: `Enum.AvatarPromptResult`)

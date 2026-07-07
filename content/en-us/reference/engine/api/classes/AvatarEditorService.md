---
title: AvatarEditorService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# AvatarEditorService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **BustAvatarFetchCache**() -> `null`
- **CheckApplyDefaultClothing**(`humanoidDescription: HumanoidDescription`) -> `HumanoidDescription` [Yields] [Deprecated]
- **CheckApplyDefaultClothingAsync**(`humanoidDescription: HumanoidDescription`) -> `HumanoidDescription` [Yields]
- **ConformToAvatarRules**(`humanoidDescription: HumanoidDescription`) -> `HumanoidDescription` [Yields] [Deprecated]
- **ConformToAvatarRulesAsync**(`humanoidDescription: HumanoidDescription`) -> `HumanoidDescription` [Yields]
- **GetAccessoryType**(`avatarAssetType: AvatarAssetType`) -> `AccessoryType`
- **GetAvatarRules**() -> `Dictionary` [Yields] [Deprecated]
- **GetAvatarRulesAsync**() -> `Dictionary` [Yields]
- **GetBatchItemDetails**(`itemIds: Array`, `itemType: AvatarItemType`) -> `Array` [Yields] [Deprecated]
- **GetBatchItemDetailsAsync**(`itemIds: Array`, `itemType: AvatarItemType`) -> `Array` [Yields]
- **GetBundlesByAssetIdAsync**(`assetId: int64`, `limit: int64 = 10`) -> `CatalogPages` [Yields]
- **GetFavorite**(`itemId: int64`, `itemType: AvatarItemType`) -> `bool` [Yields] [Deprecated]
- **GetFavoriteAsync**(`itemId: int64`, `itemType: AvatarItemType`) -> `bool` [Yields]
- **GetHeadShapesAsync**() -> `Array` [Yields]
- **GetInventory**(`assetTypes: Array`) -> `InventoryPages` [Yields] [Deprecated]
- **GetInventoryAsync**(`assetTypes: Array`) -> `InventoryPages` [Yields]
- **GetItemDetails**(`itemId: int64`, `itemType: AvatarItemType`) -> `Dictionary` [Yields] [Deprecated]
- **GetItemDetailsAsync**(`itemId: int64`, `itemType: AvatarItemType`) -> `Dictionary` [Yields]
- **GetOutfitDetails**(`outfitId: int64`) -> `Dictionary` [Yields] [Deprecated]
- **GetOutfitDetailsAsync**(`outfitId: int64`) -> `Dictionary` [Yields]
- **GetOutfits**(`outfitSource: OutfitSource = All`, `outfitType: OutfitType = All`) -> `OutfitPages` [Yields] [Deprecated]
- **GetOutfitsAsync**(`outfitSource: OutfitSource = All`, `outfitType: OutfitType = All`) -> `OutfitPages` [Yields]
- **GetRecommendedAssets**(`assetType: AvatarAssetType`, `contextAssetId: int64 = 0`) -> `Array` [Yields] [Deprecated]
- **GetRecommendedAssetsAsync**(`assetType: AvatarAssetType`, `contextAssetId: int64 = 0`) -> `Array` [Yields]
- **GetRecommendedBundles**(`bundleId: int64`) -> `Array` [Yields] [Deprecated]
- **GetRecommendedBundlesAsync**(`bundleId: int64`) -> `Array` [Yields]
- **NoPromptApplyProfileConfiguration**(`profileConfiguration: Dictionary`) -> `bool`
- **NoPromptCreateOutfit**(`humanoidDescription: HumanoidDescription`, `rigType: HumanoidRigType`, `name: string`, `gearAssetId: int64 = 0`, `outfitOptions: Dictionary = nil`, `outfitType: Variant`) -> `bool`
- **NoPromptDeleteOutfit**(`outfitId: int64`) -> `bool`
- **NoPromptRenameOutfit**(`outfitId: int64`, `name: string`) -> `bool`
- **NoPromptSaveAvatar**(`humanoidDescription: HumanoidDescription`, `rigType: HumanoidRigType`, `saveDict: Dictionary`, `gearAssetId: int64 = 0`, `profileConfiguration: Dictionary = nil`) -> `bool`
- **NoPromptSaveAvatarThumbnailCustomization**(`thumbnailType: AvatarThumbnailCustomizationType`, `emoteAssetId: int64`, `cameraDistanceScale: float`, `yRotDeg: float`, `fieldOfViewDeg: float = 0`) -> `bool`
- **NoPromptSetFavorite**(`itemId: int64`, `itemType: AvatarItemType`, `shouldFavorite: bool`) -> `bool`
- **NoPromptUpdateOutfit**(`outfitId: int64`, `humanoidDescription: HumanoidDescription`, `rigType: HumanoidRigType`, `gearAssetId: int64 = 0`, `outfitOptions: Dictionary = nil`) -> `bool`
- **PerformCreateOutfitWithDescription**(`humanoidDescription: HumanoidDescription`, `name: string`, `profileConfiguration: Dictionary = nil`) -> `null`
- **PerformDeleteOutfit**() -> `null`
- **PerformRenameOutfit**(`name: string`) -> `null`
- **PerformSaveAvatarWithDescription**(`humanoidDescription: HumanoidDescription`, `addedAssets: Array`, `removedAssets: Array`) -> `null`
- **PerformSetFavorite**() -> `null`
- **PerformUpdateOutfit**(`humanoidDescription: HumanoidDescription`, `profileConfiguration: Dictionary = nil`) -> `null`
- **PromptAllowInventoryReadAccess**() -> `null`
- **PromptCreateOutfit**(`outfit: HumanoidDescription`, `rigType: HumanoidRigType`, `outfitOptions: Dictionary = nil`, `outfitType: Variant`) -> `null`
- **PromptDeleteOutfit**(`outfitId: int64`) -> `null`
- **PromptRenameOutfit**(`outfitId: int64`) -> `null`
- **PromptSaveAvatar**(`humanoidDescription: HumanoidDescription`, `rigType: HumanoidRigType`) -> `null`
- **PromptSetFavorite**(`itemId: int64`, `itemType: AvatarItemType`, `shouldFavorite: bool`) -> `null`
- **PromptUpdateOutfit**(`outfitId: int64`, `updatedOutfit: HumanoidDescription`, `rigType: HumanoidRigType`) -> `null`
- **SearchCatalog**(`searchParameters: CatalogSearchParams`) -> `CatalogPages` [Yields] [Deprecated]
- **SearchCatalogAsync**(`searchParameters: CatalogSearchParams`) -> `CatalogPages` [Yields]
- **SetAllowInventoryReadAccess**(`inventoryReadAccessGranted: bool`) -> `null`
- **SignalCreateOutfitFailed**() -> `null`
- **SignalCreateOutfitPermissionDenied**() -> `null`
- **SignalDeleteOutfitFailed**() -> `null`
- **SignalDeleteOutfitPermissionDenied**() -> `null`
- **SignalRenameOutfitFailed**() -> `null`
- **SignalRenameOutfitPermissionDenied**() -> `null`
- **SignalSaveAvatarFailed**() -> `null`
- **SignalSaveAvatarPermissionDenied**() -> `null`
- **SignalSetFavoriteFailed**() -> `null`
- **SignalSetFavoritePermissionDenied**() -> `null`
- **SignalUpdateOutfitFailed**() -> `null`
- **SignalUpdateOutfitPermissionDenied**() -> `null`
- **refreshAvatarThumbnails**(`thumbnailTypes: Array`) -> `null`

## Events

- **OpenAllowInventoryReadAccess**()
- **OpenPromptCreateOufit**(`humanoidDescription: HumanoidDescription`, `rigType: HumanoidRigType`)
- **OpenPromptDeleteOutfit**(`outfitId: int64`)
- **OpenPromptRenameOutfit**(`outfitId: int64`)
- **OpenPromptSaveAvatar**(`humanoidDescription: HumanoidDescription`, `rigType: HumanoidRigType`)
- **OpenPromptSetFavorite**(`itemId: int64`, `itemType: AvatarItemType`, `shouldFavorite: bool`)
- **OpenPromptUpdateOutfit**(`outfitId: int64`, `humanoidDescription: HumanoidDescription`, `rigType: HumanoidRigType`)
- **PromptAllowInventoryReadAccessCompleted**(`result: AvatarPromptResult`)
- **PromptApplyProfileConfigurationCompleted**(`result: AvatarPromptResult`)
- **PromptCreateOutfitCompleted**(`result: AvatarPromptResult`, `failureType: Variant`)
- **PromptDeleteOutfitCompleted**(`result: AvatarPromptResult`)
- **PromptRenameOutfitCompleted**(`result: AvatarPromptResult`)
- **PromptSaveAvatarCompleted**(`result: AvatarPromptResult`, `humanoidDescription: HumanoidDescription`)
- **PromptSaveAvatarThumbnailCustomizationCompleted**(`result: AvatarPromptResult`, `failureType: Variant`)
- **PromptSetFavoriteCompleted**(`result: AvatarPromptResult`)
- **PromptUpdateOutfitCompleted**(`result: AvatarPromptResult`)

---
title: AvatarEditorService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# AvatarEditorService

A service to support developer Avatar Editors.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

AvatarEditorService is a service to support developer Avatar Editors. It
provides methods to modify the player's platform avatar, request information
about a user's inventory, and request information about the catalog.

For more information regarding the Avatar Editor, see
[Avatar Editor Service](../../../players/avatar-editor.md).

#### Throttling

The following endpoints on `AvatarEditorService` have experience-level
throttling:

- `Class.AvatarEditorService.GetItemDetailsAsync`
- `Class.AvatarEditorService.GetBatchItemDetailsAsync`
- `Class.AvatarEditorService.GetRecommendedAssetsAsync`
- `Class.AvatarEditorService.GetRecommendedBundlesAsync`
- `Class.AvatarEditorService.SearchCatalogAsync`
- `Class.AvatarEditorService.PromptSetFavorite`
- `Class.AvatarEditorService.GetFavoriteAsync`

For each experience, this throttling allows you to send up to 100 requests per
second to these `AvatarEditorService` endpoints, regardless of the number of
servers or user count. Exceeding these limits returns a
`429 Too Many Requests` error.

#### Item Details Response

The following methods return item data in a shared response format:

- `Class.AvatarEditorService:GetItemDetailsAsync()`
- `Class.AvatarEditorService:GetBatchItemDetailsAsync()`
- `Class.AvatarEditorService:GetBundlesByAssetIdAsync()`
- `Class.AvatarEditorService:SearchCatalogAsync()`

```lua
{
  "Id": 0,
  "ItemType": "Asset",
  "AssetType": "Image",
  "BundleType": "BodyParts",
  "Name": "string",
  "Description": "string",
  "ProductId": 0,
  "ItemStatus": ["New"],
  "ItemRestrictions": ["Collectible"],

  "BundledItems": [
    {
      "Id": 0,
      "Name": "string",
      "Type": "Asset",
      "AssetType": "string",
      "SupportsHeadShapes": false,
      "Owned": false
    }
  ],
  "IsRecolorable": false,

  "CollectibleItemId": "string",
  "TotalQuantity": 0,
  "UnitsAvailableForConsumption": 0,
  "QuantityLimitPerUser": 0,
  "HasResellers": false,
  "OffSaleDeadline": null,

  "Price": 0,
  "PremiumPricing": {
    "PremiumDiscountPercentage": 0,
    "PremiumPriceInRobux": 0
  },
  "LowestPrice": 0,
  "LowestResalePrice": 0,
  "PriceStatus": "string",
  "SaleLocationType": "ShopAndAllExperiences",
  "PurchaseCount": 0,
  "FavoriteCount": 0,

  "CreatorType": "User",
  "CreatorTargetId": 0,
  "CreatorName": "string",
  "CreatorHasVerifiedBadge": false,

  "SupportsHeadShapes": false,

  "TimedOptions": [
    { "Duration": 259200, "Price": 30 },
    { "Duration": 604800, "Price": 40 },
    { "Duration": 1209600, "Price": 50 }
  ]
}
```

##### Basic Information

<table>
  <thead>
    <tr>
      <th>Field</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
  <tr>
    <td><code>Id</code></td>
    <td>number</td>
    <td>The unique identifier of the item.</td>
  </tr>
  <tr>
    <td><code>ItemType</code></td>
    <td>string</td>
    <td>The type of item: <code>"Asset"</code> or <code>"Bundle"</code>. Corresponds to <code>Enum.AvatarItemType</code>.</td>
  </tr>
  <tr>
    <td><code>AssetType</code></td>
    <td>string</td>
    <td>The asset type. Corresponds to <code>Enum.AvatarAssetType</code> values (e.g., <code>"Hat"</code>, <code>"Shirt"</code>). Only present if <code>ItemType</code> is <code>"Asset"</code>.</td>
  </tr>
  <tr>
    <td><code>SupportsHeadShapes</code></td>
    <td>boolean</td>
    <td>Whether the asset supports head shape swapping. Only present if <code>AssetType</code> is <code>"DynamicHead"</code>.</td>
  </tr>
  <tr>
    <td><code>BundleType</code></td>
    <td>string</td>
    <td>The bundle type. Corresponds to <code>Enum.BundleType</code> values (e.g., <code>"BodyParts"</code>, <code>"Animations"</code>). Only present if <code>ItemType</code> is <code>"Bundle"</code>.</td>
  </tr>
  <tr>
    <td><code>Name</code></td>
    <td>string</td>
    <td>The display name of the item.</td>
  </tr>
  <tr>
    <td><code>Description</code></td>
    <td>string</td>
    <td>The item's description text.</td>
  </tr>
  <tr>
    <td><code>ProductId</code></td>
    <td>number</td>
    <td>The product ID associated with this item.</td>
  </tr>
  <tr>
    <td><code>ItemStatus</code></td>
    <td>array</td>
    <td>An array of status strings (e.g., <code>"New"</code>, <code>"Sale"</code>, <code>"XboxExclusive"</code>, <code>"AmazonExclusive"</code>).</td>
  </tr>
  <tr>
    <td><code>ItemRestrictions</code></td>
    <td>array</td>
    <td>An array of restriction strings. See the <code>itemRestrictions</code> table below.</td>
  </tr>
  </tbody>
</table>

##### Bundle Information

<table>
  <thead>
    <tr>
      <th>Field</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
  <tr>
    <td><code>BundledItems</code></td>
    <td>array</td>
    <td>An array of items contained in the bundle. Only present if <code>ItemType</code> is <code>"Bundle"</code>. Each entry contains:</td>
  </tr>
  <tr>
    <td colspan="2"></td>
    <td><code>Id</code>: The unique identifier of the bundled item.</td>
  </tr>
  <tr>
    <td colspan="2"></td>
    <td><code>Name</code>: The display name of the bundled item.</td>
  </tr>
  <tr>
    <td colspan="2"></td>
    <td><code>Type</code>: The type of the bundled item (e.g., <code>"Asset"</code>).</td>
  </tr>
  <tr>
    <td colspan="2"></td>
    <td><code>AssetType</code>: The asset type as a string. Corresponds to <code>Enum.AvatarAssetType</code> values (e.g., <code>"Hat"</code>, <code>"DynamicHead"</code>).</td>
  </tr>
  <tr>
    <td colspan="2"></td>
    <td><code>SupportsHeadShapes</code>: Whether the asset supports head shape swapping. Only present if <code>AssetType</code> is <code>"DynamicHead"</code>.</td>
  </tr>
  <tr>
    <td colspan="2"></td>
    <td><code>Owned</code>: Whether the bundled item is owned by the current user.</td>
  </tr>
  <tr>
    <td><code>IsRecolorable</code></td>
    <td>boolean</td>
    <td>Whether the bundle supports skin tone matching. Only applies to BodyParts and DynamicHead bundles.</td>
  </tr>
  </tbody>
</table>

##### Collectible Information

<table>
  <thead>
    <tr>
      <th>Field</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
  <tr>
    <td><code>CollectibleItemId</code></td>
    <td>string</td>
    <td>The unique item ID of the collectible.</td>
  </tr>
  <tr>
    <td><code>TotalQuantity</code></td>
    <td>number</td>
    <td>The total quantity of the collectible available for purchase (not resale).</td>
  </tr>
  <tr>
    <td><code>UnitsAvailableForConsumption</code></td>
    <td>number</td>
    <td>The number of units available for purchase. Only applies to Limited items with remaining stock.</td>
  </tr>
  <tr>
    <td><code>QuantityLimitPerUser</code></td>
    <td>number</td>
    <td>Maximum number of the same collectible item a user can own.</td>
  </tr>
  <tr>
    <td><code>HasResellers</code></td>
    <td>boolean</td>
    <td><code>true</code> when item is a Limited collectible and there are copies available for resale.</td>
  </tr>
  <tr>
    <td><code>OffSaleDeadline</code></td>
    <td>string</td>
    <td>The date/time when the item goes off sale.</td>
  </tr>
  </tbody>
</table>

##### Pricing and Sale Information

<table>
  <thead>
    <tr>
      <th>Field</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
  <tr>
    <td><code>Price</code></td>
    <td>number</td>
    <td>The price in Robux. <code>0</code> if free or not for sale.</td>
  </tr>
  <tr>
    <td><code>PremiumPricing</code></td>
    <td>table</td>
    <td>Premium pricing information. Contains the following fields:</td>
  </tr>
  <tr>
    <td colspan="2"></td>
    <td><code>PremiumDiscountPercentage</code>: The discount percentage for Premium members.</td>
  </tr>
  <tr>
    <td colspan="2"></td>
    <td><code>PremiumPriceInRobux</code>: The discounted price in Robux for Premium members.</td>
  </tr>
  <tr>
    <td><code>LowestPrice</code></td>
    <td>number</td>
    <td>The lowest resale price for Limited items.</td>
  </tr>
  <tr>
    <td><code>LowestResalePrice</code></td>
    <td>number</td>
    <td>The lowest resale price for the collectible in Robux.</td>
  </tr>
  <tr>
    <td><code>PriceStatus</code></td>
    <td>string</td>
    <td>The price status (e.g., <code>"Free"</code>, <code>"Off Sale"</code>, <code>"No Resellers"</code>).</td>
  </tr>
  <tr>
    <td><code>SaleLocationType</code></td>
    <td>string</td>
    <td>The type of sale location setting. See <code>SaleLocationType</code> values below.</td>
  </tr>
  <tr>
    <td><code>PurchaseCount</code></td>
    <td>number</td>
    <td>The total number of times this item has been purchased.</td>
  </tr>
  <tr>
    <td><code>FavoriteCount</code></td>
    <td>number</td>
    <td>The total number of users who have favorited this item.</td>
  </tr>
  </tbody>
</table>

##### Creator Information

<table>
  <thead>
    <tr>
      <th>Field</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
  <tr>
    <td><code>CreatorType</code></td>
    <td>string</td>
    <td>Either <code>User</code> or <code>Group</code>. See <code>Enum.CreatorType</code>.</td>
  </tr>
  <tr>
    <td><code>CreatorTargetId</code></td>
    <td>number</td>
    <td>The ID of the creator user or group.</td>
  </tr>
  <tr>
    <td><code>CreatorName</code></td>
    <td>string</td>
    <td>The display name of the creator.</td>
  </tr>
  <tr>
    <td><code>CreatorHasVerifiedBadge</code></td>
    <td>boolean</td>
    <td>Boolean of whether the creator has a verified badge.</td>
  </tr>
  </tbody>
</table>

##### Timed Options Information

<table>
  <thead>
    <tr>
      <th>Field</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
  <tr>
    <td><code>TimedOptions</code></td>
    <td>array</td>
    <td>Optional. An array of available timed options with durations and prices. Only present for assets that support timed ownership. Do not hardcode duration values; always retrieve them from the API as available options may change. Each entry contains:</td>
  </tr>
  <tr>
    <td colspan="2"></td>
    <td><code>Duration</code>: The duration in seconds (e.g. 259200 for 3 days, 604800 for 7 days).</td>
  </tr>
  <tr>
    <td colspan="2"></td>
    <td><code>Price</code>: The price in Robux for this duration.</td>
  </tr>
  </tbody>
</table>

##### SaleLocationType Values

| Value                    | Description                                                                            |
| :----------------------- | :------------------------------------------------------------------------------------- |
| `NotApplicable`          | Default value, should not occur in practice.                                           |
| `ShopOnly`               | Item can only be purchased in the Roblox catalog shop.                                 |
| `MyExperiencesOnly`      | Item can only be purchased in the creator's experiences.                               |
| `ShopAndMyExperiences`   | Item can be purchased in the Roblox catalog shop or the creator's experiences.         |
| `ExperiencesById`        | Item can only be purchased in a specific list of experiences.                          |
| `ShopAndAllExperiences`  | Item can be purchased in the Roblox catalog shop and all experiences.                  |
| `ExperiencesDevApiOnly`  | Item can only be purchased in experiences via developer APIs.                          |
| `ShopAndExperiencesById` | Item can be purchased in the Roblox catalog shop or a whitelisted list of experiences. |

##### itemRestrictions Values

| itemRestrictions | Limited or Unlimited  |
| :--------------: | :-------------------: |
|     `empty`      |       Unlimited       |
|  `Collectible`   |      UGC Limited      |
|    `Limited`     |    Roblox Limited     |
| `LimitedUnique`  | Roblox Limited Unique |

## Methods

### `Class.AvatarEditorService:BustAvatarFetchCache`

``BustAvatarFetchCache()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:CheckApplyDefaultClothing`

``CheckApplyDefaultClothing(humanoidDescription: `Class.HumanoidDescription`)`` -> `Class.HumanoidDescription`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:CheckApplyDefaultClothingAsync`

``CheckApplyDefaultClothingAsync(humanoidDescription: `Class.HumanoidDescription`)`` -> `Class.HumanoidDescription`
  [Yields]

### `Class.AvatarEditorService:ConformToAvatarRules`

``ConformToAvatarRules(humanoidDescription: `Class.HumanoidDescription`)`` -> `Class.HumanoidDescription`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:ConformToAvatarRulesAsync`

``ConformToAvatarRulesAsync(humanoidDescription: `Class.HumanoidDescription`)`` -> `Class.HumanoidDescription`
  [Yields]

### `Class.AvatarEditorService:GetAccessoryType`

``GetAccessoryType(avatarAssetType: `Enum.AvatarAssetType`)`` -> `Enum.AccessoryType`

### `Class.AvatarEditorService:GetAvatarRules`

``GetAvatarRules()`` -> `Dictionary`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:GetAvatarRulesAsync`

``GetAvatarRulesAsync()`` -> `Dictionary`
  [Yields]

### `Class.AvatarEditorService:GetBatchItemDetails`

``GetBatchItemDetails(itemIds: `Array`, itemType: `Enum.AvatarItemType`)`` -> `Array`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:GetBatchItemDetailsAsync`

``GetBatchItemDetailsAsync(itemIds: `Array`, itemType: `Enum.AvatarItemType`)`` -> `Array`
  [Yields]

### `Class.AvatarEditorService:GetBundlesByAssetIdAsync`

``GetBundlesByAssetIdAsync(assetId: `int64`, limit: `int64`)`` -> `Class.CatalogPages`
  [Yields]

### `Class.AvatarEditorService:GetFavorite`

``GetFavorite(itemId: `int64`, itemType: `Enum.AvatarItemType`)`` -> `bool`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:GetFavoriteAsync`

``GetFavoriteAsync(itemId: `int64`, itemType: `Enum.AvatarItemType`)`` -> `bool`
  [Yields]

### `Class.AvatarEditorService:GetHeadShapesAsync`

``GetHeadShapesAsync()`` -> `Array`
  [Yields]

### `Class.AvatarEditorService:GetInventory`

``GetInventory(assetTypes: `Array`)`` -> `Class.InventoryPages`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:GetInventoryAsync`

``GetInventoryAsync(assetTypes: `Array`)`` -> `Class.InventoryPages`
  [Yields]

### `Class.AvatarEditorService:GetItemDetails`

``GetItemDetails(itemId: `int64`, itemType: `Enum.AvatarItemType`)`` -> `Dictionary`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:GetItemDetailsAsync`

``GetItemDetailsAsync(itemId: `int64`, itemType: `Enum.AvatarItemType`)`` -> `Dictionary`
  [Yields]

### `Class.AvatarEditorService:GetOutfitDetails`

``GetOutfitDetails(outfitId: `int64`)`` -> `Dictionary`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:GetOutfitDetailsAsync`

``GetOutfitDetailsAsync(outfitId: `int64`)`` -> `Dictionary`
  [Yields]

### `Class.AvatarEditorService:GetOutfits`

``GetOutfits(outfitSource: `Enum.OutfitSource`, outfitType: `Enum.OutfitType`)`` -> `Class.OutfitPages`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:GetOutfitsAsync`

``GetOutfitsAsync(outfitSource: `Enum.OutfitSource`, outfitType: `Enum.OutfitType`)`` -> `Class.OutfitPages`
  [Yields]

### `Class.AvatarEditorService:GetRecommendedAssets`

``GetRecommendedAssets(assetType: `Enum.AvatarAssetType`, contextAssetId: `int64`)`` -> `Array`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:GetRecommendedAssetsAsync`

``GetRecommendedAssetsAsync(assetType: `Enum.AvatarAssetType`, contextAssetId: `int64`)`` -> `Array`
  [Yields]

### `Class.AvatarEditorService:GetRecommendedBundles`

``GetRecommendedBundles(bundleId: `int64`)`` -> `Array`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:GetRecommendedBundlesAsync`

``GetRecommendedBundlesAsync(bundleId: `int64`)`` -> `Array`
  [Yields]

### `Class.AvatarEditorService:NoPromptApplyProfileConfiguration`

``NoPromptApplyProfileConfiguration(profileConfiguration: `Dictionary`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:NoPromptCreateOutfit`

``NoPromptCreateOutfit(humanoidDescription: `Class.HumanoidDescription`, rigType: `Enum.HumanoidRigType`, name: `string`, gearAssetId: `int64`, outfitOptions: `Dictionary`, outfitType: `Variant`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:NoPromptDeleteOutfit`

``NoPromptDeleteOutfit(outfitId: `int64`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:NoPromptRenameOutfit`

``NoPromptRenameOutfit(outfitId: `int64`, name: `string`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:NoPromptSaveAvatar`

``NoPromptSaveAvatar(humanoidDescription: `Class.HumanoidDescription`, rigType: `Enum.HumanoidRigType`, saveDict: `Dictionary`, gearAssetId: `int64`, profileConfiguration: `Dictionary`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:NoPromptSaveAvatarThumbnailCustomization`

``NoPromptSaveAvatarThumbnailCustomization(thumbnailType: `Enum.AvatarThumbnailCustomizationType`, emoteAssetId: `int64`, cameraDistanceScale: `float`, yRotDeg: `float`, fieldOfViewDeg: `float`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:NoPromptSetFavorite`

``NoPromptSetFavorite(itemId: `int64`, itemType: `Enum.AvatarItemType`, shouldFavorite: `bool`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:NoPromptUpdateOutfit`

``NoPromptUpdateOutfit(outfitId: `int64`, humanoidDescription: `Class.HumanoidDescription`, rigType: `Enum.HumanoidRigType`, gearAssetId: `int64`, outfitOptions: `Dictionary`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:PerformCreateOutfitWithDescription`

``PerformCreateOutfitWithDescription(humanoidDescription: `Class.HumanoidDescription`, name: `string`, profileConfiguration: `Dictionary`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:PerformDeleteOutfit`

``PerformDeleteOutfit()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:PerformRenameOutfit`

``PerformRenameOutfit(name: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:PerformSaveAvatarWithDescription`

``PerformSaveAvatarWithDescription(humanoidDescription: `Class.HumanoidDescription`, addedAssets: `Array`, removedAssets: `Array`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:PerformSetFavorite`

``PerformSetFavorite()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:PerformUpdateOutfit`

``PerformUpdateOutfit(humanoidDescription: `Class.HumanoidDescription`, profileConfiguration: `Dictionary`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:PromptAllowInventoryReadAccess`

``PromptAllowInventoryReadAccess()`` -> `null`

### `Class.AvatarEditorService:PromptCreateOutfit`

``PromptCreateOutfit(outfit: `Class.HumanoidDescription`, rigType: `Enum.HumanoidRigType`, outfitOptions: `Dictionary`, outfitType: `Variant`)`` -> `null`

### `Class.AvatarEditorService:PromptDeleteOutfit`

``PromptDeleteOutfit(outfitId: `int64`)`` -> `null`

### `Class.AvatarEditorService:PromptRenameOutfit`

``PromptRenameOutfit(outfitId: `int64`)`` -> `null`

### `Class.AvatarEditorService:PromptSaveAvatar`

``PromptSaveAvatar(humanoidDescription: `Class.HumanoidDescription`, rigType: `Enum.HumanoidRigType`)`` -> `null`

### `Class.AvatarEditorService:PromptSetFavorite`

``PromptSetFavorite(itemId: `int64`, itemType: `Enum.AvatarItemType`, shouldFavorite: `bool`)`` -> `null`

### `Class.AvatarEditorService:PromptUpdateOutfit`

``PromptUpdateOutfit(outfitId: `int64`, updatedOutfit: `Class.HumanoidDescription`, rigType: `Enum.HumanoidRigType`)`` -> `null`

### `Class.AvatarEditorService:SearchCatalog`

``SearchCatalog(searchParameters: `Datatype.CatalogSearchParams`)`` -> `Class.CatalogPages`
  [Yields] [Deprecated]

### `Class.AvatarEditorService:SearchCatalogAsync`

``SearchCatalogAsync(searchParameters: `Datatype.CatalogSearchParams`)`` -> `Class.CatalogPages`
  [Yields]

### `Class.AvatarEditorService:SetAllowInventoryReadAccess`

``SetAllowInventoryReadAccess(inventoryReadAccessGranted: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalCreateOutfitFailed`

``SignalCreateOutfitFailed()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalCreateOutfitPermissionDenied`

``SignalCreateOutfitPermissionDenied()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalDeleteOutfitFailed`

``SignalDeleteOutfitFailed()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalDeleteOutfitPermissionDenied`

``SignalDeleteOutfitPermissionDenied()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalRenameOutfitFailed`

``SignalRenameOutfitFailed()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalRenameOutfitPermissionDenied`

``SignalRenameOutfitPermissionDenied()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalSaveAvatarFailed`

``SignalSaveAvatarFailed()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalSaveAvatarPermissionDenied`

``SignalSaveAvatarPermissionDenied()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalSetFavoriteFailed`

``SignalSetFavoriteFailed()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalSetFavoritePermissionDenied`

``SignalSetFavoritePermissionDenied()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalUpdateOutfitFailed`

``SignalUpdateOutfitFailed()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:SignalUpdateOutfitPermissionDenied`

``SignalUpdateOutfitPermissionDenied()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AvatarEditorService:refreshAvatarThumbnails`

``refreshAvatarThumbnails(thumbnailTypes: `Array`)`` -> `null`
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

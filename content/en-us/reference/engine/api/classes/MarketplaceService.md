---
title: MarketplaceService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# MarketplaceService

The service responsible for in-experience transactions.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

`Class.MarketplaceService` is responsible for in-experience transactions. The
most notable methods are
`Class.MarketplaceService:PromptProductPurchase()|PromptProductPurchase` and
`Class.MarketplaceService:PromptPurchase()|PromptPurchase`, as well as the
callback `Class.MarketplaceService.ProcessReceipt|ProcessReceipt` which must
be defined so that developer product transactions do not fail.

`Class.MarketplaceService` also has methods that fetch information about
[developer products](../../../production/monetization/developer-products.md)
(`Class.MarketplaceService:GetProductInfoAsync()|GetProductInfoAsync` and
`Class.MarketplaceService:GetDeveloperProductsAsync()|GetDeveloperProductsAsync`),
[passes](../../../production/monetization/passes.md)
(`Class.MarketplaceService:UserOwnsGamePassAsync()|UserOwnsGamePassAsync()`),
and other assets
(`Class.MarketplaceService:PlayerOwnsAssetAsync()|PlayerOwnsAssetAsync`,
`Class.MarketplaceService:PlayerOwnsBundleAsync()|PlayerOwnsBundleAsync`).

Understanding `Class.MarketplaceService` is the first step towards learning to
[monetize](../../../production/monetization/index.md) an experience on Roblox,
as well as learning to use `Class.DataStoreService`, which is responsible for
saving and loading all data related to purchases.

## Methods

### `Class.MarketplaceService:BindReceiptHandler`

``BindReceiptHandler(transactionType: `Enum.ReceiptType`, handler: `Datatype.Function`, filter: `Array?`)`` -> `Datatype.RBXScriptConnection`

### `Class.MarketplaceService:ClearProductInfoCaches`

``ClearProductInfoCaches()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:GetAvailableSubscriptionProductsAsync`

``GetAvailableSubscriptionProductsAsync(productType: `string`)`` -> `Array`
  [Yields] {security: RobloxScriptSecurity}

### `Class.MarketplaceService:GetDeveloperProductsAsync`

``GetDeveloperProductsAsync()`` -> `Class.Instance`
  [Yields]

### `Class.MarketplaceService:GetProductInfo`

``GetProductInfo(assetId: `int64`, infoType: `Enum.InfoType`)`` -> `Dictionary`
  [Yields] [Deprecated]

### `Class.MarketplaceService:GetProductInfoAsync`

``GetProductInfoAsync(assetId: `int64`, infoType: `Enum.InfoType`)`` -> `Dictionary`
  [Yields]

### `Class.MarketplaceService:GetRobloxSubscriptionDetailsAsync`

``GetRobloxSubscriptionDetailsAsync(user: `Class.Player`)`` -> `Dictionary`
  [Yields]

### `Class.MarketplaceService:GetRobuxBalance`

``GetRobuxBalance()`` -> `int`
  [Yields] {security: RobloxScriptSecurity}

### `Class.MarketplaceService:GetSubscriptionProductInfoAsync`

``GetSubscriptionProductInfoAsync(subscriptionId: `string`)`` -> `Dictionary`
  [Yields]

### `Class.MarketplaceService:GetSubscriptionPurchaseInfoAsync`

``GetSubscriptionPurchaseInfoAsync(subscriptionId: `string`)`` -> `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.MarketplaceService:GetUserSubscriptionDetailsAsync`

``GetUserSubscriptionDetailsAsync(user: `Class.Player`, subscriptionId: `string`)`` -> `Dictionary`
  [Yields]

### `Class.MarketplaceService:GetUserSubscriptionDetailsInternalAsync`

``GetUserSubscriptionDetailsInternalAsync(subscriptionId: `string`)`` -> `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.MarketplaceService:GetUserSubscriptionPaymentHistoryAsync`

``GetUserSubscriptionPaymentHistoryAsync(user: `Class.Player`, subscriptionId: `string`)`` -> `Array`
  [Yields]

### `Class.MarketplaceService:GetUserSubscriptionStatusAsync`

``GetUserSubscriptionStatusAsync(user: `Class.Player`, subscriptionId: `string`)`` -> `Dictionary`
  [Yields]

### `Class.MarketplaceService:GetUsersPriceLevelsAsync`

``GetUsersPriceLevelsAsync(userIds: `Array`)`` -> `Array`
  [Yields]

### `Class.MarketplaceService:IsPurchaseSimulated`

``IsPurchaseSimulated()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:OpenShop`

``OpenShop(player: `Class.Player`)`` -> `null`

### `Class.MarketplaceService:PerformBulkPurchase`

``PerformBulkPurchase(orderRequest: `Dictionary`, options: `Dictionary`)`` -> `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.MarketplaceService:PerformCancelSubscription`

``PerformCancelSubscription(subscriptionId: `string`)`` -> `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.MarketplaceService:PerformPurchase`

``PerformPurchase(infoType: `Enum.InfoType`, productId: `int64`, expectedPrice: `int`, requestId: `string`, isRobloxPurchase: `bool`, collectibleItemId: `string`, collectibleProductId: `string`, idempotencyKey: `string`, purchaseAuthToken: `string`, timedOptionsDays: `int64`, purchasePayload: `string`, purchaseOptions: `Dictionary`)`` -> `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.MarketplaceService:PerformPurchaseV2`

``PerformPurchaseV2(infoType: `Enum.InfoType`, productId: `int64`, expectedPrice: `int`, requestId: `string`, isRobloxPurchase: `bool`, collectiblesProductDetails: `Dictionary`)`` -> `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.MarketplaceService:PerformSubscriptionPurchase`

``PerformSubscriptionPurchase(subscriptionId: `string`)`` -> `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.MarketplaceService:PerformSubscriptionPurchaseV2`

``PerformSubscriptionPurchaseV2(subscriptionId: `string`, paymentProvider: `string`)`` -> `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.MarketplaceService:PerformSubscriptionPurchaseV3Async`

``PerformSubscriptionPurchaseV3Async(productType: `string`, productId: `string`, paymentProvider: `string`, paymentSessionId: `string`)`` -> `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.MarketplaceService:PerformSubscriptionPurchaseWithRobuxAsync`

``PerformSubscriptionPurchaseWithRobuxAsync(subscriptionId: `string`, priceInRobux: `int`)`` -> `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.MarketplaceService:PlayerCanMakePurchases`

``PlayerCanMakePurchases(player: `Class.Instance`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:PlayerOwnsAsset`

``PlayerOwnsAsset(player: `Class.Instance`, assetId: `int64`)`` -> `bool`
  [Yields] [Deprecated]

### `Class.MarketplaceService:PlayerOwnsAssetAsync`

``PlayerOwnsAssetAsync(player: `Class.Instance`, assetId: `int64`)`` -> `bool`
  [Yields]

### `Class.MarketplaceService:PlayerOwnsBundle`

``PlayerOwnsBundle(player: `Class.Player`, bundleId: `int64`)`` -> `bool`
  [Yields] [Deprecated]

### `Class.MarketplaceService:PlayerOwnsBundleAsync`

``PlayerOwnsBundleAsync(player: `Class.Player`, bundleId: `int64`)`` -> `bool`
  [Yields]

### `Class.MarketplaceService:PrepareCollectiblesPurchase`

``PrepareCollectiblesPurchase(player: `Class.Instance`, assetId: `int64`, collectibleItemId: `string`, collectibleItemInstanceId: `string`, collectibleProductId: `string`, expectedPrice: `int`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:PromptBulkPurchase`

``PromptBulkPurchase(player: `Class.Player`, lineItems: `Array`, options: `Dictionary`)`` -> `null`

### `Class.MarketplaceService:PromptBundlePurchase`

``PromptBundlePurchase(player: `Class.Instance`, bundleId: `int64`)`` -> `null`

### `Class.MarketplaceService:PromptCancelSubscription`

``PromptCancelSubscription(user: `Class.Player`, subscriptionId: `string`)`` -> `null`

### `Class.MarketplaceService:PromptCollectiblesPurchase`

``PromptCollectiblesPurchase(player: `Class.Instance`, assetId: `int64`, collectibleItemId: `string`, collectibleItemInstanceId: `string`, collectibleProductId: `string`, expectedPrice: `int`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:PromptGamePassPurchase`

``PromptGamePassPurchase(player: `Class.Instance`, gamePassId: `int64`)`` -> `null`

### `Class.MarketplaceService:PromptNativePurchase`

``PromptNativePurchase(player: `Class.Instance`, productId: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:PromptNativePurchaseWithLocalPlayer`

``PromptNativePurchaseWithLocalPlayer(productId: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:PromptNativePurchaseWithLocalPlayerWithPaymentSessionId`

``PromptNativePurchaseWithLocalPlayerWithPaymentSessionId(productId: `string`, paymentSessionId: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:PromptNativePurchaseWithPaymentSessionId`

``PromptNativePurchaseWithPaymentSessionId(player: `Class.Instance`, productId: `string`, paymentSessionId: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:PromptPremiumPurchase`

``PromptPremiumPurchase(player: `Class.Instance`)`` -> `null`
  [Deprecated]

### `Class.MarketplaceService:PromptProductPurchase`

``PromptProductPurchase(player: `Class.Instance`, productId: `int64`, equipIfPurchased: `bool`, currencyType: `Enum.CurrencyType`)`` -> `null`

### `Class.MarketplaceService:PromptPurchase`

``PromptPurchase(player: `Class.Instance`, assetId: `int64`, equipIfPurchased: `bool`, currencyType: `Enum.CurrencyType`)`` -> `null`

### `Class.MarketplaceService:PromptRobloxPurchase`

``PromptRobloxPurchase(assetId: `int64`, equipIfPurchased: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:PromptRobloxSubscriptionPurchase`

``PromptRobloxSubscriptionPurchase(user: `Class.Player`)`` -> `null`

### `Class.MarketplaceService:PromptRobuxTransferAsync`

``PromptRobuxTransferAsync(sender: `Class.Player`, receiverUserId: `int64`, amount: `int64`)`` -> `string`
  [Yields]

### `Class.MarketplaceService:PromptSubscriptionPurchase`

``PromptSubscriptionPurchase(user: `Class.Player`, subscriptionId: `string`)`` -> `null`

### `Class.MarketplaceService:PromptThirdPartyPurchase`

``PromptThirdPartyPurchase(player: `Class.Instance`, productId: `string`)`` -> `null`
   {security: LocalUserSecurity}

### `Class.MarketplaceService:RankProductsAsync`

``RankProductsAsync(productIdentifiers: `Array`)`` -> `Array`
  [Yields]

### `Class.MarketplaceService:RecommendTopProductsAsync`

``RecommendTopProductsAsync(infoTypes: `Array`)`` -> `Array`
  [Yields]

### `Class.MarketplaceService:ReportAssetSale`

``ReportAssetSale(assetId: `string`, robuxAmount: `int`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:ReportRobuxUpsellStarted`

``ReportRobuxUpsellStarted()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:SignalAssetTypePurchased`

``SignalAssetTypePurchased(player: `Class.Instance`, assetType: `Enum.AssetType`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:SignalCheckPlayerHasRobloxSubscription`

``SignalCheckPlayerHasRobloxSubscription()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:SignalClientPurchaseSuccess`

``SignalClientPurchaseSuccess(ticket: `string`, playerId: `int64`, productId: `int64`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:SignalMockPurchasePremium`

``SignalMockPurchasePremium()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:SignalMockPurchaseRobloxSubscription`

``SignalMockPurchaseRobloxSubscription()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:SignalPromptBulkPurchaseFinished`

``SignalPromptBulkPurchaseFinished(status: `Enum.MarketplaceBulkPurchasePromptStatus`, results: `Dictionary`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:SignalPromptBundlePurchaseFinished`

``SignalPromptBundlePurchaseFinished(player: `Class.Instance`, bundleId: `int64`, success: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:SignalPromptGamePassPurchaseFinished`

``SignalPromptGamePassPurchaseFinished(player: `Class.Instance`, gamePassId: `int64`, success: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:SignalPromptPremiumPurchaseFinished`

``SignalPromptPremiumPurchaseFinished(didTryPurchasing: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:SignalPromptProductPurchaseFinished`

``SignalPromptProductPurchaseFinished(userId: `int64`, productId: `int64`, success: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:SignalPromptPurchaseFinished`

``SignalPromptPurchaseFinished(player: `Class.Instance`, assetId: `int64`, success: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:SignalPromptRobloxSubscriptionPurchaseFinished`

``SignalPromptRobloxSubscriptionPurchaseFinished(subscriptionId: `string`, didTryPurchasing: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:SignalPromptSubscriptionPurchaseFinished`

``SignalPromptSubscriptionPurchaseFinished(subscriptionId: `string`, didTryPurchasing: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:SignalRobuxTransferCompleted`

``SignalRobuxTransferCompleted(userId: `int64`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:SignalServerLuaDialogClosed`

``SignalServerLuaDialogClosed(value: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:SignalUserSubscriptionStatusChanged`

``SignalUserSubscriptionStatusChanged(subscriptionId: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.MarketplaceService:UserOwnsGamePassAsync`

``UserOwnsGamePassAsync(userId: `Datatype.User`, gamePassId: `int64`)`` -> `bool`
  [Yields]

## Events

### `Class.MarketplaceService.ClientLuaDialogRequested`

Fires with: (arguments: `Tuple`)

### `Class.MarketplaceService.ClientPurchaseSuccess`

Fires with: (ticket: `string`, playerId: `int64`, productId: `int64`)

### `Class.MarketplaceService.NativePurchaseFinished`

Fires with: (player: `Class.Instance`, productId: `string`, wasPurchased: `bool`)

### `Class.MarketplaceService.NativePurchaseFinishedWithLocalPlayer`

Fires with: (productId: `string`, wasPurchased: `bool`)

### `Class.MarketplaceService.OpenShopRequested`

Fires with: (player: `Class.Player`)

### `Class.MarketplaceService.PrepareCollectiblesPurchaseRequested`

Fires with: (player: `Class.Instance`, assetId: `int64`, collectibleItemId: `string`, collectibleItemInstanceId: `string`, collectibleProductId: `string`, expectedPrice: `int`)

### `Class.MarketplaceService.PromptBulkPurchaseFinished`

Fires with: (player: `Class.Instance`, status: `Enum.MarketplaceBulkPurchasePromptStatus`, results: `Dictionary`)

### `Class.MarketplaceService.PromptBulkPurchaseRequested`

Fires with: (player: `Class.Instance`, displayData: `Array`, orderRequest: `Dictionary`, purchaserRobuxBalance: `int64`, orderTotalRobux: `int64`, options: `Dictionary`)

### `Class.MarketplaceService.PromptBulkPurchaseRequestedV2`

Fires with: (player: `Class.Instance`, displayData: `Array`, orderRequest: `Dictionary`, purchaserRobuxBalance: `int64`, orderTotalRobux: `int64`, options: `Dictionary`, discountInformation: `Dictionary`)

### `Class.MarketplaceService.PromptBundlePurchaseFinished`

Fires with: (player: `Class.Instance`, bundleId: `int64`, wasPurchased: `bool`)

### `Class.MarketplaceService.PromptBundlePurchaseRequested`

Fires with: (player: `Class.Instance`, bundleId: `int64`)

### `Class.MarketplaceService.PromptCancelSubscriptionRequested`

Fires with: (subscriptionId: `string`)

### `Class.MarketplaceService.PromptCollectibleBundlePurchaseRequested`

Fires with: (player: `Class.Instance`, bundleId: `int64`, collectibleItemId: `string`, collectibleItemInstanceId: `string`, collectibleProductId: `string`, expectedPrice: `int`, idempotencyKey: `string`, purchaseAuthToken: `string`)

### `Class.MarketplaceService.PromptCollectiblesPurchaseRequested`

Fires with: (player: `Class.Instance`, assetId: `int64`, collectibleItemId: `string`, collectibleItemInstanceId: `string`, collectibleProductId: `string`, expectedPrice: `int`, idempotencyKey: `string`, purchaseAuthToken: `string`)

### `Class.MarketplaceService.PromptGamePassPurchaseFinished`

Fires with: (player: `Class.Instance`, gamePassId: `int64`, wasPurchased: `bool`)

### `Class.MarketplaceService.PromptGamePassPurchaseRequested`

Fires with: (player: `Class.Instance`, gamePassId: `int64`)

### `Class.MarketplaceService.PromptPremiumPurchaseFinished`

Fires with: ()

### `Class.MarketplaceService.PromptPremiumPurchaseRequested`

Fires with: (player: `Class.Instance`)

### `Class.MarketplaceService.PromptProductPurchaseFinished`

Fires with: (userId: `int64`, productId: `int64`, isPurchased: `bool`)

### `Class.MarketplaceService.PromptProductPurchaseRequested`

Fires with: (player: `Class.Instance`, productId: `int64`, equipIfPurchased: `bool`, currencyType: `Enum.CurrencyType`)

### `Class.MarketplaceService.PromptPurchaseFinished`

Fires with: (player: `Class.Instance`, assetId: `int64`, isPurchased: `bool`)

### `Class.MarketplaceService.PromptPurchaseRequested`

Fires with: (player: `Class.Instance`, assetId: `int64`, equipIfPurchased: `bool`, currencyType: `Enum.CurrencyType`)

### `Class.MarketplaceService.PromptPurchaseRequestedV2`

Fires with: (player: `Class.Instance`, assetId: `int64`, equipIfPurchased: `bool`, currencyType: `Enum.CurrencyType`, idempotencyKey: `string`, purchaseAuthToken: `string`)

### `Class.MarketplaceService.PromptRobloxPurchaseRequested`

Fires with: (assetId: `int64`, equipIfPurchased: `bool`)

### `Class.MarketplaceService.PromptRobloxSubscriptionPurchaseFinished`

Fires with: (user: `Class.Player`, didTryPurchasing: `bool`)

### `Class.MarketplaceService.PromptRobloxSubscriptionPurchaseRequested`

Fires with: ()

### `Class.MarketplaceService.PromptRobuxTransferRequested`

Fires with: (player: `Class.Instance`, jsonResponse: `string`)

### `Class.MarketplaceService.PromptRobuxTransferSubscriptionUpsellRequested`

Fires with: ()

### `Class.MarketplaceService.PromptSubscriptionPurchaseFinished`

Fires with: (user: `Class.Player`, subscriptionId: `string`, didTryPurchasing: `bool`)

### `Class.MarketplaceService.PromptSubscriptionPurchaseRequested`

Fires with: (subscriptionId: `string`)

### `Class.MarketplaceService.RobuxTransferCompleted`

Fires with: (userId: `int64`)

### `Class.MarketplaceService.ServerPurchaseVerification`

Fires with: (serverResponseTable: `Dictionary`)

### `Class.MarketplaceService.ThirdPartyPurchaseFinished`

Fires with: (player: `Class.Instance`, productId: `string`, receipt: `string`, wasPurchased: `bool`)

### `Class.MarketplaceService.UserSubscriptionStatusChanged`

Fires with: (subscriptionId: `string`)

## Callbacks

### `Class.MarketplaceService.ProcessReceipt`

``ProcessReceipt(receiptInfo: `Dictionary`)`` -> `Enum.ProductPurchaseDecision`

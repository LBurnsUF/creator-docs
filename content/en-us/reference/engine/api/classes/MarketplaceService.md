---
title: MarketplaceService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# MarketplaceService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **BindReceiptHandler**(`transactionType: ReceiptType`, `handler: Function`, `filter: Array?`) -> `RBXScriptConnection`
- **ClearProductInfoCaches**() -> `null`
- **GetAvailableSubscriptionProductsAsync**(`productType: string`) -> `Array` [Yields]
- **GetDeveloperProductsAsync**() -> `Instance` [Yields]
- **GetProductInfo**(`assetId: int64`, `infoType: InfoType = Asset`) -> `Dictionary` [Yields] [Deprecated]
- **GetProductInfoAsync**(`assetId: int64`, `infoType: InfoType = Asset`) -> `Dictionary` [Yields]
- **GetRobloxSubscriptionDetailsAsync**(`user: Player`) -> `Dictionary` [Yields]
- **GetRobuxBalance**() -> `int` [Yields]
- **GetSubscriptionProductInfoAsync**(`subscriptionId: string`) -> `Dictionary` [Yields]
- **GetSubscriptionPurchaseInfoAsync**(`subscriptionId: string`) -> `Dictionary` [Yields]
- **GetUserSubscriptionDetailsAsync**(`user: Player`, `subscriptionId: string`) -> `Dictionary` [Yields]
- **GetUserSubscriptionDetailsInternalAsync**(`subscriptionId: string`) -> `Dictionary` [Yields]
- **GetUserSubscriptionPaymentHistoryAsync**(`user: Player`, `subscriptionId: string`) -> `Array` [Yields]
- **GetUserSubscriptionStatusAsync**(`user: Player`, `subscriptionId: string`) -> `Dictionary` [Yields]
- **GetUsersPriceLevelsAsync**(`userIds: Array`) -> `Array` [Yields]
- **IsPurchaseSimulated**() -> `bool`
- **OpenShop**(`player: Player`) -> `null`
- **PerformBulkPurchase**(`orderRequest: Dictionary`, `options: Dictionary`) -> `Dictionary` [Yields]
- **PerformCancelSubscription**(`subscriptionId: string`) -> `null` [Yields]
- **PerformPurchase**(`infoType: InfoType`, `productId: int64`, `expectedPrice: int`, `requestId: string`, `isRobloxPurchase: bool`, `collectibleItemId: string = `, `collectibleProductId: string = `, `idempotencyKey: string = `, `purchaseAuthToken: string = `, `timedOptionsDays: int64 = 0`, `purchasePayload: string = `, `purchaseOptions: Dictionary = nil`) -> `Dictionary` [Yields]
- **PerformPurchaseV2**(`infoType: InfoType`, `productId: int64`, `expectedPrice: int`, `requestId: string`, `isRobloxPurchase: bool`, `collectiblesProductDetails: Dictionary`) -> `Dictionary` [Yields]
- **PerformSubscriptionPurchase**(`subscriptionId: string`) -> `string` [Yields]
- **PerformSubscriptionPurchaseV2**(`subscriptionId: string`, `paymentProvider: string`) -> `null` [Yields]
- **PerformSubscriptionPurchaseV3Async**(`productType: string`, `productId: string`, `paymentProvider: string`, `paymentSessionId: string`) -> `null` [Yields]
- **PerformSubscriptionPurchaseWithRobuxAsync**(`subscriptionId: string`, `priceInRobux: int`) -> `null` [Yields]
- **PlayerCanMakePurchases**(`player: Instance`) -> `bool`
- **PlayerOwnsAsset**(`player: Instance`, `assetId: int64`) -> `bool` [Yields] [Deprecated]
- **PlayerOwnsAssetAsync**(`player: Instance`, `assetId: int64`) -> `bool` [Yields]
- **PlayerOwnsBundle**(`player: Player`, `bundleId: int64`) -> `bool` [Yields] [Deprecated]
- **PlayerOwnsBundleAsync**(`player: Player`, `bundleId: int64`) -> `bool` [Yields]
- **PrepareCollectiblesPurchase**(`player: Instance`, `assetId: int64`, `collectibleItemId: string`, `collectibleItemInstanceId: string`, `collectibleProductId: string`, `expectedPrice: int`) -> `null`
- **PromptBulkPurchase**(`player: Player`, `lineItems: Array`, `options: Dictionary`) -> `null`
- **PromptBundlePurchase**(`player: Instance`, `bundleId: int64`) -> `null`
- **PromptCancelSubscription**(`user: Player`, `subscriptionId: string`) -> `null`
- **PromptCollectiblesPurchase**(`player: Instance`, `assetId: int64`, `collectibleItemId: string`, `collectibleItemInstanceId: string`, `collectibleProductId: string`, `expectedPrice: int`) -> `null`
- **PromptGamePassPurchase**(`player: Instance`, `gamePassId: int64`) -> `null`
- **PromptNativePurchase**(`player: Instance`, `productId: string`) -> `null`
- **PromptNativePurchaseWithLocalPlayer**(`productId: string`) -> `null`
- **PromptNativePurchaseWithLocalPlayerWithPaymentSessionId**(`productId: string`, `paymentSessionId: string`) -> `null`
- **PromptNativePurchaseWithPaymentSessionId**(`player: Instance`, `productId: string`, `paymentSessionId: string`) -> `null`
- **PromptPremiumPurchase**(`player: Instance`) -> `null` [Deprecated]
- **PromptProductPurchase**(`player: Instance`, `productId: int64`, `equipIfPurchased: bool = true`, `currencyType: CurrencyType = Default`) -> `null`
- **PromptPurchase**(`player: Instance`, `assetId: int64`, `equipIfPurchased: bool = true`, `currencyType: CurrencyType = Default`) -> `null`
- **PromptRobloxPurchase**(`assetId: int64`, `equipIfPurchased: bool`) -> `null`
- **PromptRobloxSubscriptionPurchase**(`user: Player`) -> `null`
- **PromptRobuxTransferAsync**(`sender: Player`, `receiverUserId: int64`, `amount: int64`) -> `string` [Yields]
- **PromptSubscriptionPurchase**(`user: Player`, `subscriptionId: string`) -> `null`
- **PromptThirdPartyPurchase**(`player: Instance`, `productId: string`) -> `null`
- **RankProductsAsync**(`productIdentifiers: Array`) -> `Array` [Yields]
- **RecommendTopProductsAsync**(`infoTypes: Array`) -> `Array` [Yields]
- **ReportAssetSale**(`assetId: string`, `robuxAmount: int`) -> `null`
- **ReportRobuxUpsellStarted**() -> `null`
- **SignalAssetTypePurchased**(`player: Instance`, `assetType: AssetType`) -> `null`
- **SignalCheckPlayerHasRobloxSubscription**() -> `null`
- **SignalClientPurchaseSuccess**(`ticket: string`, `playerId: int64`, `productId: int64`) -> `null`
- **SignalMockPurchasePremium**() -> `null`
- **SignalMockPurchaseRobloxSubscription**() -> `null`
- **SignalPromptBulkPurchaseFinished**(`status: MarketplaceBulkPurchasePromptStatus`, `results: Dictionary`) -> `null`
- **SignalPromptBundlePurchaseFinished**(`player: Instance`, `bundleId: int64`, `success: bool`) -> `null`
- **SignalPromptGamePassPurchaseFinished**(`player: Instance`, `gamePassId: int64`, `success: bool`) -> `null`
- **SignalPromptPremiumPurchaseFinished**(`didTryPurchasing: bool`) -> `null`
- **SignalPromptProductPurchaseFinished**(`userId: int64`, `productId: int64`, `success: bool`) -> `null`
- **SignalPromptPurchaseFinished**(`player: Instance`, `assetId: int64`, `success: bool`) -> `null`
- **SignalPromptRobloxSubscriptionPurchaseFinished**(`subscriptionId: string`, `didTryPurchasing: bool`) -> `null`
- **SignalPromptSubscriptionPurchaseFinished**(`subscriptionId: string`, `didTryPurchasing: bool`) -> `null`
- **SignalRobuxTransferCompleted**(`userId: int64`) -> `null`
- **SignalServerLuaDialogClosed**(`value: bool`) -> `null`
- **SignalUserSubscriptionStatusChanged**(`subscriptionId: string`) -> `null`
- **UserOwnsGamePassAsync**(`userId: User`, `gamePassId: int64`) -> `bool` [Yields]

## Events

- **ClientLuaDialogRequested**(`arguments: Tuple`)
- **ClientPurchaseSuccess**(`ticket: string`, `playerId: int64`, `productId: int64`)
- **NativePurchaseFinished**(`player: Instance`, `productId: string`, `wasPurchased: bool`)
- **NativePurchaseFinishedWithLocalPlayer**(`productId: string`, `wasPurchased: bool`)
- **OpenShopRequested**(`player: Player`)
- **PrepareCollectiblesPurchaseRequested**(`player: Instance`, `assetId: int64`, `collectibleItemId: string`, `collectibleItemInstanceId: string`, `collectibleProductId: string`, `expectedPrice: int`)
- **PromptBulkPurchaseFinished**(`player: Instance`, `status: MarketplaceBulkPurchasePromptStatus`, `results: Dictionary`)
- **PromptBulkPurchaseRequested**(`player: Instance`, `displayData: Array`, `orderRequest: Dictionary`, `purchaserRobuxBalance: int64`, `orderTotalRobux: int64`, `options: Dictionary`)
- **PromptBulkPurchaseRequestedV2**(`player: Instance`, `displayData: Array`, `orderRequest: Dictionary`, `purchaserRobuxBalance: int64`, `orderTotalRobux: int64`, `options: Dictionary`, `discountInformation: Dictionary`)
- **PromptBundlePurchaseFinished**(`player: Instance`, `bundleId: int64`, `wasPurchased: bool`)
- **PromptBundlePurchaseRequested**(`player: Instance`, `bundleId: int64`)
- **PromptCancelSubscriptionRequested**(`subscriptionId: string`)
- **PromptCollectibleBundlePurchaseRequested**(`player: Instance`, `bundleId: int64`, `collectibleItemId: string`, `collectibleItemInstanceId: string`, `collectibleProductId: string`, `expectedPrice: int`, `idempotencyKey: string`, `purchaseAuthToken: string`)
- **PromptCollectiblesPurchaseRequested**(`player: Instance`, `assetId: int64`, `collectibleItemId: string`, `collectibleItemInstanceId: string`, `collectibleProductId: string`, `expectedPrice: int`, `idempotencyKey: string`, `purchaseAuthToken: string`)
- **PromptGamePassPurchaseFinished**(`player: Instance`, `gamePassId: int64`, `wasPurchased: bool`)
- **PromptGamePassPurchaseRequested**(`player: Instance`, `gamePassId: int64`)
- **PromptPremiumPurchaseFinished**()
- **PromptPremiumPurchaseRequested**(`player: Instance`)
- **PromptProductPurchaseFinished**(`userId: int64`, `productId: int64`, `isPurchased: bool`)
- **PromptProductPurchaseRequested**(`player: Instance`, `productId: int64`, `equipIfPurchased: bool`, `currencyType: CurrencyType`)
- **PromptPurchaseFinished**(`player: Instance`, `assetId: int64`, `isPurchased: bool`)
- **PromptPurchaseRequested**(`player: Instance`, `assetId: int64`, `equipIfPurchased: bool`, `currencyType: CurrencyType`)
- **PromptPurchaseRequestedV2**(`player: Instance`, `assetId: int64`, `equipIfPurchased: bool`, `currencyType: CurrencyType`, `idempotencyKey: string`, `purchaseAuthToken: string`)
- **PromptRobloxPurchaseRequested**(`assetId: int64`, `equipIfPurchased: bool`)
- **PromptRobloxSubscriptionPurchaseFinished**(`user: Player`, `didTryPurchasing: bool`)
- **PromptRobloxSubscriptionPurchaseRequested**()
- **PromptRobuxTransferRequested**(`player: Instance`, `jsonResponse: string`)
- **PromptRobuxTransferSubscriptionUpsellRequested**()
- **PromptSubscriptionPurchaseFinished**(`user: Player`, `subscriptionId: string`, `didTryPurchasing: bool`)
- **PromptSubscriptionPurchaseRequested**(`subscriptionId: string`)
- **RobuxTransferCompleted**(`userId: int64`)
- **ServerPurchaseVerification**(`serverResponseTable: Dictionary`)
- **ThirdPartyPurchaseFinished**(`player: Instance`, `productId: string`, `receipt: string`, `wasPurchased: bool`)
- **UserSubscriptionStatusChanged**(`subscriptionId: string`)

## Callbacks

- **ProcessReceipt**(`receiptInfo: Dictionary`) -> `ProductPurchaseDecision`

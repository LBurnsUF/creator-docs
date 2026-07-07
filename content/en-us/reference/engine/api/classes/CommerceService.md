---
title: CommerceService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# CommerceService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **GetCommerceProductInfoAsync**(`commerceProductId: string`) -> `Dictionary` [Yields]
- **PrepareCommerceProductPurchase**(`commerceProductId: string`) -> `Dictionary` [Yields]
- **PromptCommerceProductPurchase**(`user: Player`, `commerceProductId: string`) -> `null`
- **PromptRealWorldCommerceBrowser**(`player: Player`, `url: string`) -> `null`
- **SignalPromptCommerceProductPurchaseFinished**(`productId: string`, `didTryPurchase: bool`, `checkoutSessionId: string = `) -> `null`
- **UserEligibleForRealWorldCommerceAsync**() -> `bool` [Yields]

## Events

- **BenefitStatusReceived**(`isGranted: bool`)
- **FetchReceipt**()
- **InExperienceBrowserRequested**(`url: string`)
- **PromptCommerceProductPurchaseFinished**(`user: Player`, `productId: string`)
- **PromptCommerceProductPurchaseRequested**(`commerceProductId: string`)
- **PurchaseBrowserClosed**()

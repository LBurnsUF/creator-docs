---
title: CommerceService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# CommerceService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.CommerceService:GetCommerceProductInfoAsync`

``GetCommerceProductInfoAsync(commerceProductId: `string`)`` → `Dictionary`
  [Yields]

### `Class.CommerceService:PrepareCommerceProductPurchase`

``PrepareCommerceProductPurchase(commerceProductId: `string`)`` → `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.CommerceService:PromptCommerceProductPurchase`

``PromptCommerceProductPurchase(user: `Class.Player`, commerceProductId: `string`)`` → `null`

### `Class.CommerceService:PromptRealWorldCommerceBrowser`

``PromptRealWorldCommerceBrowser(player: `Class.Player`, url: `string`)`` → `null`

### `Class.CommerceService:SignalPromptCommerceProductPurchaseFinished`

``SignalPromptCommerceProductPurchaseFinished(productId: `string`, didTryPurchase: `bool`, checkoutSessionId: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.CommerceService:UserEligibleForRealWorldCommerceAsync`

``UserEligibleForRealWorldCommerceAsync()`` → `bool`
  [Yields]

## Events

### `Class.CommerceService.BenefitStatusReceived`

Fires with: (isGranted: `bool`)

### `Class.CommerceService.FetchReceipt`

Fires with: ()

### `Class.CommerceService.InExperienceBrowserRequested`

Fires with: (url: `string`)

### `Class.CommerceService.PromptCommerceProductPurchaseFinished`

Fires with: (user: `Class.Player`, productId: `string`)

### `Class.CommerceService.PromptCommerceProductPurchaseRequested`

Fires with: (commerceProductId: `string`)

### `Class.CommerceService.PurchaseBrowserClosed`

Fires with: ()

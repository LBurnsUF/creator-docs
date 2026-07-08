---
title: CommerceService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# CommerceService

Supports real-world purchases that you can bundle with digital benefits.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

`Class.CommerceService` is a service that supports real-world purchases that
you can bundle with virtual items. For information on eligibility and
implementation, see
[Commerce products](../../../production/monetization/commerce-products.md).

## Methods

### `Class.CommerceService:GetCommerceProductInfoAsync`

``GetCommerceProductInfoAsync(commerceProductId: `string`)`` -> `Dictionary`
  [Yields]

### `Class.CommerceService:PrepareCommerceProductPurchase`

``PrepareCommerceProductPurchase(commerceProductId: `string`)`` -> `Dictionary`
  [Yields] {security: RobloxScriptSecurity}

### `Class.CommerceService:PromptCommerceProductPurchase`

``PromptCommerceProductPurchase(user: `Class.Player`, commerceProductId: `string`)`` -> `null`

### `Class.CommerceService:PromptRealWorldCommerceBrowser`

``PromptRealWorldCommerceBrowser(player: `Class.Player`, url: `string`)`` -> `null`

### `Class.CommerceService:SignalPromptCommerceProductPurchaseFinished`

``SignalPromptCommerceProductPurchaseFinished(productId: `string`, didTryPurchase: `bool`, checkoutSessionId: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CommerceService:UserEligibleForRealWorldCommerceAsync`

``UserEligibleForRealWorldCommerceAsync()`` -> `bool`
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

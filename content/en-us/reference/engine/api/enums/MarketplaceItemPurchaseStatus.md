---
title: MarketplaceItemPurchaseStatus
type: enum
---

# `Enum.MarketplaceItemPurchaseStatus`

The status of the item purchase through MarketplaceService.

The status of the item purchase through MarketplaceService.

The `Enum.MarketplaceItemPurchaseStatus` enum has 13 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.MarketplaceItemPurchaseStatus.Success` | 1 | The item is purchased successfully. |
| `Enum.MarketplaceItemPurchaseStatus.SystemError` | 2 | Unable to purchase item due to Roblox system error. |
| `Enum.MarketplaceItemPurchaseStatus.AlreadyOwned` | 3 | Unable to purchase item because user already owns the item. Users can only own one copy of non-limit |
| `Enum.MarketplaceItemPurchaseStatus.InsufficientRobux` | 4 | Unable to purchase item because of insufficient Robux. |
| `Enum.MarketplaceItemPurchaseStatus.QuantityLimitExceeded` | 5 | User has reached the max quantity allowed per user set by the creator for limited items. |
| `Enum.MarketplaceItemPurchaseStatus.QuotaExceeded` | 6 | The user has exceeded our [purchase request limit](../../../marketplace/marketplace-fees-and-commiss |
| `Enum.MarketplaceItemPurchaseStatus.NotForSale` | 7 | Item is not for sale. |
| `Enum.MarketplaceItemPurchaseStatus.NotAvailableForPurchaser` | 8 | This item is restricted to a group of users and the purchaser is not in this group. |
| `Enum.MarketplaceItemPurchaseStatus.PriceMismatch` | 9 | The provided price does not match the item price. Most likely the price changed since displayed to t |
| `Enum.MarketplaceItemPurchaseStatus.SoldOut` | 10 | The item is sold out. |
| `Enum.MarketplaceItemPurchaseStatus.PurchaserIsSeller` | 11 | The purchaser is the same user as the seller, for a resale purchase. |
| `Enum.MarketplaceItemPurchaseStatus.InsufficientMembership` | 12 | The user does not have sufficient premium membership to purchase this item. |
| `Enum.MarketplaceItemPurchaseStatus.PlaceInvalid` | 13 | The item is not allowed to be sold in the place. |

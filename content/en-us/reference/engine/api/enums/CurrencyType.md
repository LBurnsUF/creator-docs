---
title: CurrencyType
type: enum
---

# `Enum.CurrencyType`

The CurrencyType Enum is used with `Class.MarketplaceService` to set the
currency used.

The CurrencyType Enum is used with `Class.MarketplaceService` to set the
currency used. As tickets no longer exist on the Roblox platform, this enum is
**ignored** in most API that previously used it, such as
`Class.MarketplaceService:PromptPurchase()|PromptPurchase`.

The `Enum.CurrencyType` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.CurrencyType.Default` | 0 |  |
| `Enum.CurrencyType.Robux` | 1 | Use Robux. |
| `Enum.CurrencyType.Tix` | 2 | Use Tickets. |

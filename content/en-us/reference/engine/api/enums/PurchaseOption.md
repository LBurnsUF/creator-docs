---
title: PurchaseOption
type: enum
---

# `Enum.PurchaseOption`

Specifies the type of purchase option in a bulk purchase prompt.

The `Enum.PurchaseOption` enum specifies the type of purchase option when
building the `PurchaseOptions` array for
`Class.MarketplaceService:PromptBulkPurchase()`.

Use `TimedOption` for timed option durations and `Permanent` for standard
full-price purchase. Only one entry is allowed in `PurchaseOptions`; providing
more than one throws an error.

Do not hardcode duration values when using `TimedOption`. Always retrieve
available durations from the backend APIs and pass them through, as they may
change at any time.

The `Enum.PurchaseOption` enum has 2 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.PurchaseOption.TimedOption` | 1 | A timed ownership option. The `Value` field specifies the duration in seconds. |
| `Enum.PurchaseOption.Permanent` | 2 | A permanent ownership purchase option. |

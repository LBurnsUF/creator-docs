---
title: ReceiptDecision
type: enum
---

# `Enum.ReceiptDecision`

`ReceiptDecision` works with `Class.MarketplaceService` to indicate the
acknowledgement of receipts.

`ReceiptDecision` is the required return type for callbacks registered with
`Class.MarketplaceService:BindReceiptHandler()`. The value you return
determines whether the receipt is marked as complete or remains unresolved for
future processing.

The `Enum.ReceiptDecision` enum has 2 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ReceiptDecision.NotProcessedYet` | 0 | The receipt has not been processed yet. Returning this value keeps the receipt unresolved so it will |
| `Enum.ReceiptDecision.Processed` | 1 | The receipt has been processed and all benefits have been granted. The receipt is marked as complete |

---
title: ReceiptType
type: enum
---

# `Enum.ReceiptType`

`ReceiptType` is used to work with server-sided receipt processing.

`ReceiptType` works with `Class.MarketplaceService:BindReceiptHandler()` to
indicate the different type of receipts a developer can bind to for
processing. When you call
`Class.MarketplaceService:BindReceiptHandler()|BindReceiptHandler`, you pass a
`ReceiptType` to specify which kind of receipt your handler should process.

For Robux transfers initiated with
`Class.MarketplaceService:PromptRobuxTransferAsync()|PromptRobuxTransferAsync`,
two receipts are generated: one for the sender (`RobuxTransferSender`) and one
for the receiver (`RobuxTransferReceiver`). You should register handlers for
both types to fully process a transfer.

Transfer receipts are delivered to whichever server the user is currently in
once the transfer settles (the user does not need to rejoin). If the user is
offline when the transfer settles, the receipt is delivered the next time they
join a server. See
`Class.MarketplaceService:BindReceiptHandler()|BindReceiptHandler` for
details.

The `Enum.ReceiptType` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ReceiptType.DeveloperProduct` | 0 |  |
| `Enum.ReceiptType.RobuxTransferSender` | 1 | Used for processing receipts for the user who initiated a Robux transfer. The receipt's `PlayerId` i |
| `Enum.ReceiptType.RobuxTransferReceiver` | 2 | Used for processing receipts for the user who received Robux via a transfer. The receipt's `PlayerId |

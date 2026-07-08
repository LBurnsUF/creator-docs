---
title: MarketplaceBulkPurchasePromptStatus
type: enum
---

# `Enum.MarketplaceBulkPurchasePromptStatus`

The status of the BulkPurchasePrompt after player interaction.

The status of the BulkPurchasePrompt after player interaction.

The `Enum.MarketplaceBulkPurchasePromptStatus` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.MarketplaceBulkPurchasePromptStatus.Completed` | 1 | User confirmed the purchase and the transaction has been processed. |
| `Enum.MarketplaceBulkPurchasePromptStatus.Aborted` | 2 | User closed the prompt. |
| `Enum.MarketplaceBulkPurchasePromptStatus.Error` | 3 | User confirmed the purchase, but the transaction cannot be sent to the backend for processing. |

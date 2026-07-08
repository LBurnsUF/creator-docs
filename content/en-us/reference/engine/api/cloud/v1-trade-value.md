---
title: V1 / Trade Value
type: cloud-api
tags: [Accounts]
---

# V1 / Trade Value

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/trade-value` | Get a user's trade quality filter setting |
| `POST` | `/v1/trade-value` | Updates a user's trade quality filter setting |

### `GET` `/v1/trade-value`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

### `POST` `/v1/trade-value`

**Responses:**

- `200` - OK
- `400` - Roblox.AccountSettings.Api.ResponseEnums.TradeSettingsErrors.InvalidTradeValue
- `401` - 0: Authorization has been denied for this request.
- `403` - Roblox.AccountSettings.Api.ResponseEnums.TradeSettingsErrors.AccountLocked             OR         

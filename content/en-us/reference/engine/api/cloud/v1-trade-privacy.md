---
title: V1 / Trade Privacy
type: cloud-api
tags: [Accounts]
---

# V1 / Trade Privacy

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/trade-privacy` | Get a user's trade privacy setting |
| `POST` | `/v1/trade-privacy` | Updates a user's trade privacy setting |

### `GET` `/v1/trade-privacy`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

### `POST` `/v1/trade-privacy`

**Responses:**

- `200` - OK
- `400` - Roblox.AccountSettings.Api.ResponseEnums.TradeSettingsErrors.InvalidTradePrivacy
- `401` - 0: Authorization has been denied for this request.
- `403` - Roblox.AccountSettings.Api.ResponseEnums.TradeSettingsErrors.AccountLocked             OR         

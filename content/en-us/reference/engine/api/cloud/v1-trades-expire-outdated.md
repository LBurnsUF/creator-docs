---
title: V1 / Trades / Expire Outdated
type: cloud-api
tags: [Trades]
---

# V1 / Trades / Expire Outdated

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/trades/expire-outdated` | Deprecated. TradeSession are automatically set to expire while the inbound/outbound trades are fetch |

### `POST` `/v1/trades/expire-outdated`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

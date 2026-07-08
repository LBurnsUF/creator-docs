---
title: V2 / Trades / Send
type: cloud-api
tags: [Trades]
---

# V2 / Trades / Send

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v2/trades/send` | Sends a new trade. |

### `POST` `/v2/trades/send`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request. 4: You are not authorized to modify this trade.
- `403` - 0: Token Validation Failed
- `404` - 0: An unknown error occured.

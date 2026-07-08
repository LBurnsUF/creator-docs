---
title: V2 / Trades
type: cloud-api
tags: [Trades]
---

# V2 / Trades

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/trades/{tradeId}` | Gets the details of a trade. |
| `POST` | `/v2/trades/{tradeId}/counter` | Counters an existing trade. |

### `GET` `/v2/trades/{tradeId}`

**Parameters:**

- `tradeId` (path, integer (required)) - The id of the trade.

**Responses:**

- `200` - OK
- `400` - 0: An unknown error occured.
- `401` - 0: Authorization has been denied for this request. 4: You are not authorized to modify this trade.
- `403` - 4: You are not authorized to modify this trade.
- `404` - 0: An unknown error occured.

### `POST` `/v2/trades/{tradeId}/counter`

**Parameters:**

- `tradeId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request. 4: You are not authorized to modify this trade.
- `403` - 0: Token Validation Failed
- `404` - 0: An unknown error occured.

---
title: V1 / Trades
type: cloud-api
tags: [Trades]
---

# V1 / Trades

Cloud API resource group with 6 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/trades/{tradeId}` | Gets detailed information about a trade. |
| `POST` | `/v1/trades/{tradeId}/accept` | Accepts a trade. |
| `POST` | `/v1/trades/{tradeId}/counter` | Counters a trade. |
| `POST` | `/v1/trades/{tradeId}/decline` | Declines a trade. |
| `GET` | `/v1/trades/{tradeStatusType}` | Fetches a list of the authenticated user's trades. |
| `GET` | `/v1/trades/{tradeStatusType}/count` | Gets the total number of pending trades for the authenticated user. Inbound is the only accepted tr |

### `GET` `/v1/trades/{tradeId}`

**Parameters:**

- `tradeId` (path, integer (required)) - The trade id.

**Responses:**

- `200` - OK
- `400` - 2: The trade cannot be found or you are not authorized to view it.
- `401` - 0: Authorization has been denied for this request. 4: You are not authorized to modify this trade.
- `404` - 2: The trade cannot be found or you are not authorized to view it.
- `500` - 0: An unknown error occured.

### `POST` `/v1/trades/{tradeId}/accept`

**Parameters:**

- `tradeId` (path, integer (required)) - The trade id.

**Responses:**

- `200` - OK
- `400` - 2: The trade cannot be found or you are not authorized to view it. 3: The trade is inactive. 4: Yo
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `503` - 5: Trading system is unavailable

### `POST` `/v1/trades/{tradeId}/counter`

**Parameters:**

- `tradeId` (path, integer (required)) - The trade id.

**Responses:**

- `200` - OK
- `400` - 2: The trade cannot be found or you are not authorized to view it. 4: You are not authorized to mod
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `429` - 14: You are sending too many trade requests. Please slow down and try again later.
- `502` - 0: An unknown error occured.
- `503` - 5: Trading system is unavailable

### `POST` `/v1/trades/{tradeId}/decline`

**Parameters:**

- `tradeId` (path, integer (required)) - The trade id.

**Responses:**

- `200` - OK
- `400` - 2: The trade cannot be found or you are not authorized to view it. 3: The trade is inactive. 4: Yo
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `503` - 5: Trading system is unavailable

### `GET` `/v1/trades/{tradeStatusType}`

**Parameters:**

- `tradeStatusType` (path, integer (required)) - The trade status type.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - Sorted by trade creation date

**Responses:**

- `200` - OK
- `400` - 1: Invalid trade status type.
- `401` - 0: Authorization has been denied for this request.

### `GET` `/v1/trades/{tradeStatusType}/count`

**Parameters:**

- `tradeStatusType` (path, integer (required)) - The trade status type to fetch a total count for.

**Responses:**

- `200` - OK
- `400` - 1: Invalid trade status type.
- `401` - 0: Authorization has been denied for this request.

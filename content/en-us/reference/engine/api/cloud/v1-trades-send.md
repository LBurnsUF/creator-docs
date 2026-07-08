---
title: V1 / Trades / Send
type: cloud-api
tags: [Trades]
---

# V1 / Trades / Send

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/trades/send` | Sends a trade. |

### `POST` `/v1/trades/send`

**Responses:**

- `200` - OK
- `400` - 7: The user cannot trade. See field for whether the user who cannot trade is the sender or receiver.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `429` - 14: You are sending too many trade requests. Please slow down and try again later.
- `502` - 0: An unknown error occured.
- `503` - 5: Trading system is unavailable

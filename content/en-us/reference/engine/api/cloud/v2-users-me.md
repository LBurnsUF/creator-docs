---
title: V2 / Users / Me
type: cloud-api
tags: [Trades]
---

# V2 / Users / Me

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/users/me/can-trade` | Checks if the calling user can trade with others. |

### `GET` `/v2/users/me/can-trade`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request. 4: You are not authorized to modify this trade.

---
title: V1 / Phone
type: cloud-api
tags: [Accounts]
---

# V1 / Phone

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/phone` | Get Verified Phone Number |
| `POST` | `/v1/phone` | Set Phone Number |

### `GET` `/v1/phone`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `500` - 0: An unknown error occured.

### `POST` `/v1/phone`

**Responses:**

- `200` - OK
- `400` - 2: Invalid Phone Number 3: Phone Number Already Associated 8: Invalid Phone Number Type
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 5: Incorrect Password 10: 
- `429` - 6: Flooded
- `500` - 0: An unknown error occured.
- `503` - 1: This feature is currently disabled. Please try again later.

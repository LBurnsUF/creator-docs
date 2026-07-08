---
title: V1 / User / Currency
type: cloud-api
tags: [Localization]
---

# V1 / User / Currency

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/user/currency` | Gets currency for the authenticated user. |

### `GET` `/v1/user/currency`

Currency can only be retrieved for the authenticated user.

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 1: The user is invalid.

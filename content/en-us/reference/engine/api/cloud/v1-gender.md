---
title: V1 / Gender
type: cloud-api
tags: [Accounts]
---

# V1 / Gender

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/gender` | Get the user's gender **DEPRECATED** |
| `POST` | `/v1/gender` | Update the user's gender **DEPRECATED** |

### `GET` `/v1/gender`

> **Deprecated**

Replaced by users.roblox.com/v1/gender

**Responses:**

- `200` - OK
- `400` - 1: User not found.
- `401` - 0: Authorization has been denied for this request.

### `POST` `/v1/gender`

> **Deprecated**

Replaced by users.roblox.com/v1/gender

**Request Body:** The Roblox.AccountInformation.Api.Models.GenderRequest

**Responses:**

- `200` - OK
- `400` - 1: User not found. 6: The gender provided is invalid.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `500` - 0: An unknown error occured.

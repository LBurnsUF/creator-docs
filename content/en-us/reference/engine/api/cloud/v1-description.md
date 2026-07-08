---
title: V1 / Description
type: cloud-api
tags: [Accounts, User profiles]
---

# V1 / Description

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/description` | Get the user's description **DEPRECATED** |
| `POST` | `/v1/description` | Update the user's description **DEPRECATED** |

### `GET` `/v1/description`

> **Deprecated**

Replaced by users.roblox.com/v1/description

**Responses:**

- `200` - OK
- `400` - 1: User not found.
- `401` - 0: Authorization has been denied for this request.

### `POST` `/v1/description`

> **Deprecated**

Replaced by users.roblox.com/v1/description

**Request Body:** The Roblox.AccountInformation.Api.Models.DescriptionRequest

**Responses:**

- `200` - OK
- `400` - 1: User not found.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `500` - 0: An unknown error occured.
- `503` - 3: This feature is currently disabled. Please try again later.

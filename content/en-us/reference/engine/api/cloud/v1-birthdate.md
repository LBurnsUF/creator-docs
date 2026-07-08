---
title: V1 / Birthdate
type: cloud-api
tags: [Accounts]
---

# V1 / Birthdate

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/birthdate` | Get the user's birthdate **DEPRECATED** |
| `POST` | `/v1/birthdate` | Update the user's birthdate |

### `GET` `/v1/birthdate`

> **Deprecated**

Replaced by users.roblox.com/v1/birthdate

**Responses:**

- `200` - OK
- `400` - 1: User not found.
- `401` - 0: Authorization has been denied for this request.

### `POST` `/v1/birthdate`

**Request Body:** The Roblox.Users.Api.BirthdateRequest

**Responses:**

- `200` - OK
- `400` - 1: User not found. 4: The birthdate provided is invalid. 8: Password is incorrect.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: PIN is locked. 5: Invalid birthdate change.
- `500` - 0: An unknown error occured. 5: Invalid birthdate change.

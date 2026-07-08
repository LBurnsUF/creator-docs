---
title: V1 / Gender#Usersapi
type: cloud-api
tags: [Accounts]
---

# V1 / Gender#Usersapi

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/gender#UsersApi` | Get the user's gender |
| `POST` | `/v1/gender#UsersApi` | Update the user's gender |

### `GET` `/v1/gender#UsersApi`

**Responses:**

- `200` - OK
- `400` - 1: User not found.
- `401` - 0: Authorization has been denied for this request.

### `POST` `/v1/gender#UsersApi`

**Request Body:** The Roblox.Users.Api.GenderRequest

**Responses:**

- `200` - OK
- `400` - 1: User not found. 6: The gender provided is invalid.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: PIN is locked.
- `500` - 0: An unknown error occured.

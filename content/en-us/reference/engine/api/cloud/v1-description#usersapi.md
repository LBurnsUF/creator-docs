---
title: V1 / Description#Usersapi
type: cloud-api
tags: [Accounts, User profiles]
---

# V1 / Description#Usersapi

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/description#UsersApi` | Get the user's description |
| `POST` | `/v1/description#UsersApi` | Update the user's description |

### `GET` `/v1/description#UsersApi`

**Responses:**

- `200` - OK
- `400` - 1: User not found.
- `401` - 0: Authorization has been denied for this request.

### `POST` `/v1/description#UsersApi`

**Request Body:** The Roblox.Users.Api.DescriptionRequest

**Responses:**

- `200` - OK
- `400` - 1: User not found.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: PIN is locked.
- `500` - 0: An unknown error occured.
- `503` - 3: This feature is currently disabled. Please try again later.

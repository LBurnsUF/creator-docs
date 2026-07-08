---
title: V1 / User
type: cloud-api
tags: [Connections]
---

# V1 / User

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/user/{userId}/multiget-are-friends` | Check if the requesting user is friends with the specified users. |

### `POST` `/v1/user/{userId}/multiget-are-friends`

**Parameters:**

- `userId` (path, integer (required)) - The requesting userId.

**Request Body:** The user ids to check against with the requesting user.

**Responses:**

- `200` - OK
- `400` - 1: The target user is invalid or does not exist.
- `403` - 0: Token Validation Failed

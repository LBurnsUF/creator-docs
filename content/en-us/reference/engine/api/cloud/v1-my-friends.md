---
title: V1 / My / Friends
type: cloud-api
tags: [Connections]
---

# V1 / My / Friends

Cloud API resource group with 4 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/my/friends/count` | Get the number of friends a user has |
| `POST` | `/v1/my/friends/refresh-qr-session` |  |
| `GET` | `/v1/my/friends/requests` | Get all users that friend requests with targetUserId using exclusive start paging |
| `GET` | `/v1/my/friends/{userId}/check-qr-session` |  |

### `GET` `/v1/my/friends/count`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

### `POST` `/v1/my/friends/refresh-qr-session`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

### `GET` `/v1/my/friends/requests`

**Parameters:**

- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sessionId` (query, string) - Optional session identifier.
- `friendRequestSort` (query, integer) - 

**Responses:**

- `200` - OK
- `400` - 1: The target user is invalid or does not exist. 6: Invalid parameters.
- `401` - 0: Authorization has been denied for this request.
- `403` - 2: The user is banned from performing operation. 3: The user is blocked from performing this action
- `429` - 9: The flood limit has been exceeded.

### `GET` `/v1/my/friends/{userId}/check-qr-session`

**Parameters:**

- `userId` (path, integer (required)) - user Id that shows the qr code

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

---
title: V1 / Messages
type: cloud-api
tags: [Accounts]
---

# V1 / Messages

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/messages` | Gets a user's messages. |
| `GET` | `/v1/messages/{messageId}` | Gets a message's details. |

### `GET` `/v1/messages`

**Parameters:**

- `pageNumber` (query, integer) - 
- `pageSize` (query, integer) - 
- `messageTab` (query, string) - 

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

### `GET` `/v1/messages/{messageId}`

**Parameters:**

- `messageId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 2: Message does not exist or the current user is not authorized to view it.
- `401` - 0: Authorization has been denied for this request.

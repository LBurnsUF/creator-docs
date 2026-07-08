---
title: V1 / User / Friend Requests
type: cloud-api
tags: [Connections]
---

# V1 / User / Friend Requests

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/user/friend-requests/count` | Return the number of pending friend requests. |

### `GET` `/v1/user/friend-requests/count`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

---
title: V1 / Messages / Unread
type: cloud-api
tags: [Accounts]
---

# V1 / Messages / Unread

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/messages/unread/count` | Gets unread messages for the authenticated user. |

### `GET` `/v1/messages/unread/count`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

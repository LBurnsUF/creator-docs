---
title: V1 / Announcements
type: cloud-api
tags: [Accounts]
---

# V1 / Announcements

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/announcements` | Migrate from RobloxWebsite project, return news notification for Private Message page |

### `GET` `/v1/announcements`

**Responses:**

- `200` - OK
- `400` - 2: Message does not exist or the current user is not authorized to view it.
- `401` - 0: Authorization has been denied for this request.

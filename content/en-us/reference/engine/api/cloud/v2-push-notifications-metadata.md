---
title: V2 / Push Notifications / Metadata
type: cloud-api
tags: [Metadata, Notifications]
---

# V2 / Push Notifications / Metadata

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/push-notifications/metadata` | Gets the corresponding metadata for the specified notification |

### `GET` `/v2/push-notifications/metadata`

**Parameters:**

- `notificationToken` (query, string (required)) - Token for the notification
- `notificationId` (query, string (required)) - Id of the specified notification

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

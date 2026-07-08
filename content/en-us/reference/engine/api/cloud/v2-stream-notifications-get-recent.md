---
title: V2 / Stream Notifications / Get Recent
type: cloud-api
tags: [Notifications]
---

# V2 / Stream Notifications / Get Recent

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/stream-notifications/get-recent` | Gets the recent entries from the notification stream |

### `GET` `/v2/stream-notifications/get-recent`

**Parameters:**

- `startIndex` (query, integer) - Index to start the entries from. (Optional : Defaults to 0 which means the most recent entry)
- `maxRows` (query, integer) - Number of entries to be returned. (Optional : Defaults to 10 entries)

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

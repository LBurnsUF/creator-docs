---
title: V2 / Stream Notifications / Get Latest Game Updates
type: cloud-api
tags: [Notifications, Universes]
---

# V2 / Stream Notifications / Get Latest Game Updates

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/stream-notifications/get-latest-game-updates` | Get the latest non aggregated Game Updates sent to the logged in user |

### `GET` `/v2/stream-notifications/get-latest-game-updates`

**Parameters:**

- `universeIds` (query, array (required)) - List of universe IDs
- `sinceDateTime` (query, string) - For retrieving only updates that created after a time point.

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

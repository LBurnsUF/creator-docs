---
title: V2 / Avatar / Avatar
type: cloud-api
tags: [Avatars]
---

# V2 / Avatar / Avatar

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/avatar/avatar` | Returns details about the authenticated user's avatar. |

### `GET` `/v2/avatar/avatar`

**Parameters:**

- `Roblox-Place-Id` (header, integer) - 
- `checkAssetAvailability` (query, boolean) - Whether to return assets with availability status.

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

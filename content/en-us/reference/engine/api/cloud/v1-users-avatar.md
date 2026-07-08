---
title: V1 / Users / Avatar
type: cloud-api
tags: [Avatars, Thumbnails]
---

# V1 / Users / Avatar

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/users/avatar` | Get Avatar Full body shots for the given CSV of userIds [STABLE] |

### `GET` `/v1/users/avatar`

**Stability:** STABLE

**Parameters:**

- `userIds` (query, array (required)) - CSV for the userIds to get avatar full body shots
- `includeBackground` (query, boolean) - Whether to include a background in the thumbnail (defaults to false)
- `size` (query, string) - The thumbnail size, formatted widthxheight
- `format` (query, string) - The thumbnail format
- `isCircular` (query, boolean) - The circle thumbnail output parameter, true or false

**Responses:**

- `200` - OK
- `400` - 1: There are too many requested Ids. 2: The requested image format is invalid. Please see documenta

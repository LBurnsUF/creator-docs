---
title: V1 / Users / Avatar Headshot
type: cloud-api
tags: [Avatars, Thumbnails]
---

# V1 / Users / Avatar Headshot

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/users/avatar-headshot` | Get Avatar Headshots for the given CSV of userIds [STABLE] |

### `GET` `/v1/users/avatar-headshot`

**Stability:** STABLE

**Parameters:**

- `userIds` (query, array (required)) - CSV for the userIds to get avatar headshots
- `includeBackground` (query, boolean) - Whether to include a background in the thumbnail (defaults to false)
- `size` (query, string) - The thumbnail size, formatted widthxheight
- `format` (query, string) - The thumbnail format
- `isCircular` (query, boolean) - The circle thumbnail output parameter, true or false

**Responses:**

- `200` - OK
- `400` - 1: There are too many requested Ids. 2: The requested image format is invalid. Please see documenta

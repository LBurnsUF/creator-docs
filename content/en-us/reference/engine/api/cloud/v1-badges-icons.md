---
title: V1 / Badges / Icons
type: cloud-api
tags: [Badges, Thumbnails]
---

# V1 / Badges / Icons

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/badges/icons` | Thumbnails badge icons. [STABLE] |

### `GET` `/v1/badges/icons`

**Stability:** STABLE

**Parameters:**

- `badgeIds` (query, array (required)) - The badge ids.
- `size` (query, string) - The thumbnail size, formatted widthxheight
- `format` (query, string) - The thumbnail format
- `isCircular` (query, boolean) - The circle thumbnail output parameter, true or false

**Responses:**

- `200` - OK
- `400` - 1: There are too many requested Ids. 2: The requested image format is invalid. Please see documenta

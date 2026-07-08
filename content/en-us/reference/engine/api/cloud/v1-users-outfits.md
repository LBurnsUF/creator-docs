---
title: V1 / Users / Outfits
type: cloud-api
tags: [Thumbnails]
---

# V1 / Users / Outfits

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/users/outfits` | Get outfits for the given CSV of userOutfitIds [STABLE] |

### `GET` `/v1/users/outfits`

**Stability:** STABLE

**Parameters:**

- `userOutfitIds` (query, array (required)) - CSV for the userOutfitIds to get user outfits
- `includeBackground` (query, boolean) - Whether to include a background in the thumbnail (defaults to false)
- `size` (query, string) - The thumbnail size, formatted widthxheight
- `format` (query, string) - The thumbnail format
- `isCircular` (query, boolean) - The circle thumbnail output parameter, true or false

**Responses:**

- `200` - OK
- `400` - 1: There are too many requested Ids. 2: The requested image format is invalid. Please see documenta

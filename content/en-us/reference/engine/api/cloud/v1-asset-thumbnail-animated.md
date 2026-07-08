---
title: V1 / Asset Thumbnail Animated
type: cloud-api
tags: [Assets, Thumbnails]
---

# V1 / Asset Thumbnail Animated

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/asset-thumbnail-animated` | Thumbnails asset animated. [STABLE] |

### `GET` `/v1/asset-thumbnail-animated`

**Stability:** STABLE

**Parameters:**

- `assetId` (query, integer (required)) - The asset id.
- `Roblox-Place-Id` (header, integer) - (optional) placeid

**Responses:**

- `200` - OK
- `400` - 4: The requested Ids are invalid, of an invalid type or missing.

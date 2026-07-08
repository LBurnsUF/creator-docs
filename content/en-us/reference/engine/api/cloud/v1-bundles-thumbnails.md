---
title: V1 / Bundles / Thumbnails
type: cloud-api
tags: [Avatars, Thumbnails]
---

# V1 / Bundles / Thumbnails

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/bundles/thumbnails` | Get bundle thumbnails for the given CSV of bundle ids [STABLE] |

### `GET` `/v1/bundles/thumbnails`

**Stability:** STABLE

**Parameters:**

- `bundleIds` (query, array (required)) - CSV for the bundle ids to get bundle thumbnails
- `size` (query, string) - The thumbnail size, formatted widthxheight
- `format` (query, string) - The thumbnail format
- `isCircular` (query, boolean) - The circle thumbnail output parameter, true or false

**Responses:**

- `200` - OK
- `400` - 1: There are too many requested Ids. 2: The requested image format is invalid. Please see documenta

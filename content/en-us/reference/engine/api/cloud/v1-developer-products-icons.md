---
title: V1 / Developer Products / Icons
type: cloud-api
tags: [Developer products, Thumbnails]
---

# V1 / Developer Products / Icons

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/developer-products/icons` | Thumbnails developer product icons. [STABLE] |

### `GET` `/v1/developer-products/icons`

**Stability:** STABLE

**Parameters:**

- `developerProductIds` (query, array (required)) - The developer product ids.
- `size` (query, string) - The thumbnail size, formatted widthxheight
- `format` (query, string) - The thumbnail format
- `isCircular` (query, boolean) - The circle thumbnail output parameter, true or false

**Responses:**

- `200` - OK
- `400` - 1: There are too many requested Ids. 2: The requested image format is invalid. Please see documenta

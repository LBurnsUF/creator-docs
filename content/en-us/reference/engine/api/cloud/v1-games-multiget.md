---
title: V1 / Games / Multiget
type: cloud-api
tags: [Thumbnails, Universes]
---

# V1 / Games / Multiget

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/games/multiget/thumbnails` | Fetch game thumbnail URLs for a list of universe IDs. [STABLE] |

### `GET` `/v1/games/multiget/thumbnails`

**Stability:** STABLE

**Parameters:**

- `universeIds` (query, array (required)) - comma-delimited list of universe IDs
- `countPerUniverse` (query, integer) - max number of thumbnails to return per universe
- `defaults` (query, boolean) - true if defaults (if any) should be returned if no media exists
- `size` (query, string) - The thumbnail size, formatted widthxheight
- `format` (query, string) - The thumbnail format
- `isCircular` (query, boolean) - The circle thumbnail output parameter, true or false

**Responses:**

- `200` - OK
- `400` - 0: Unknown error 1: There are too many requested Ids. 4: The requested Ids are invalid, of an inva

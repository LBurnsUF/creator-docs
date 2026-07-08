---
title: V1 / Groups / Icons
type: cloud-api
tags: [Groups, Thumbnails]
---

# V1 / Groups / Icons

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/groups/icons` | Fetches thumbnail URLs for a list of groups. Ids that do not correspond to groups will be filtered o [STABLE] |

### `GET` `/v1/groups/icons`

**Stability:** STABLE

**Parameters:**

- `groupIds` (query, array (required)) - 
- `size` (query, string) - The thumbnail size, formatted widthxheight
- `format` (query, string) - The thumbnail format
- `isCircular` (query, boolean) - The circle thumbnail output parameter, true or false

**Responses:**

- `200` - OK
- `400` - 1: There are too many requested Ids. 2: The requested image format is invalid. Please see documenta

---
title: V1 / Resize
type: cloud-api
tags: [Thumbnails]
---

# V1 / Resize

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/resize/{hash}/{width}/{height}/{type}/{format}/{filterType}` | Resizes larger thumbnails to specified size and format |

### `GET` `/v1/resize/{hash}/{width}/{height}/{type}/{format}/{filterType}`

**Parameters:**

- `hash` (path, string (required)) - Hash of larger thumbnail
- `width` (path, integer (required)) - Desired width of thumbnail
- `height` (path, integer (required)) - Desired height of thumbnail
- `type` (path, string (required)) - Thumbnail Type
- `format` (path, string (required)) - Desired image format of the thumbnail
- `filterType` (query, string (required)) - E.g. is output circular
- `shouldModify` (query, boolean) - 

**Responses:**

- `200` - OK

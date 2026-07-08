---
title: V1 / Secureresize
type: cloud-api
tags: [Thumbnails]
---

# V1 / Secureresize

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/secureresize/{thumbPrint}/{hash}/{width}/{height}/{type}/{format}/{filterType}` | Decrypts and Resizes larger thumbnails to specified size and format |

### `GET` `/v1/secureresize/{thumbPrint}/{hash}/{width}/{height}/{type}/{format}/{filterType}`

**Parameters:**

- `thumbPrint` (path, string (required)) - The thumbPrint that represents the key version
- `hash` (path, string (required)) - Hash of larger thumbnail
- `width` (path, integer (required)) - Desired width of thumbnail
- `height` (path, integer (required)) - Desired height of thumbnail
- `type` (path, string (required)) - Thumbnail Type
- `format` (path, string (required)) - Desired image format of the thumbnail
- `filterType` (query, string) - E.g. is output circular

**Responses:**

- `200` - OK

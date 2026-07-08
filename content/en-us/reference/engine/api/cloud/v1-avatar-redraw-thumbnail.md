---
title: V1 / Avatar / Redraw Thumbnail
type: cloud-api
tags: [Avatars, Thumbnails, User profiles]
---

# V1 / Avatar / Redraw Thumbnail

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/avatar/redraw-thumbnail` | Requests the authenticated user's thumbnail be redrawn. |

### `POST` `/v1/avatar/redraw-thumbnail`

**Parameters:**

- `Roblox-Place-Id` (header, integer) - 

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `429` - 1: Redrawing your avatar thumbnail is floodchecked at this time. 1: Redrawing your avatar thumbnail

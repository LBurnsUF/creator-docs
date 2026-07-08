---
title: V1 / Avatar
type: cloud-api
tags: [Avatars]
---

# V1 / Avatar

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/avatar` | Returns details about the authenticated user's avatar. |

### `GET` `/v1/avatar`

**Parameters:**

- `Roblox-Place-Id` (header, integer) - 

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

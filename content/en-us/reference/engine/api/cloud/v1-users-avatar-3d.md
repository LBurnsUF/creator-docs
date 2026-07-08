---
title: V1 / Users / Avatar 3D
type: cloud-api
tags: [Avatars, Thumbnails]
---

# V1 / Users / Avatar 3D

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/users/avatar-3d` | Get Avatar 3d object for a user [BETA] |

### `GET` `/v1/users/avatar-3d`

**Stability:** BETA

**Parameters:**

- `userId` (query, integer (required)) - user Id for avatar

**Responses:**

- `200` - OK
- `400` - 4: The requested Ids are invalid, of an invalid type or missing.

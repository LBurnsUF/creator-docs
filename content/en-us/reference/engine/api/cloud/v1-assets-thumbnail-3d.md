---
title: V1 / Assets Thumbnail 3D
type: cloud-api
tags: [Assets, Thumbnails]
---

# V1 / Assets Thumbnail 3D

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/assets-thumbnail-3d` | Thumbnails assets. [BETA] |

### `GET` `/v1/assets-thumbnail-3d`

**Stability:** BETA

**Parameters:**

- `assetId` (query, integer (required)) - The asset id.
- `useGltf` (query, boolean) - (optional) formatType
- `Roblox-Place-Id` (header, integer) - (optional) placeid

**Responses:**

- `200` - OK
- `400` - 4: The requested Ids are invalid, of an invalid type or missing.

---
title: V1 / Favorites / Assets
type: cloud-api
tags: [Assets, Avatars, Interactions]
---

# V1 / Favorites / Assets

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/favorites/assets/{assetId}/count` | Gets the favorite count for the given asset Id. |

### `GET` `/v1/favorites/assets/{assetId}/count`

**Parameters:**

- `assetId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 2: Invalid asset Id.

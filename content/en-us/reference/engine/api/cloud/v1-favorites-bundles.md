---
title: V1 / Favorites / Bundles
type: cloud-api
tags: [Assets, Avatars, Interactions]
---

# V1 / Favorites / Bundles

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/favorites/bundles/{bundleId}/count` | Gets the favorite count for the given bundle Id. |

### `GET` `/v1/favorites/bundles/{bundleId}/count`

**Parameters:**

- `bundleId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 2: Invalid bundle Id.

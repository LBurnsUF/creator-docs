---
title: V1 / Bundles
type: cloud-api
tags: [Assets, Avatars]
---

# V1 / Bundles

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/bundles/{bundleId}/details` | Returns details about the given bundleId. |
| `GET` | `/v1/bundles/{bundleId}/recommendations` | Gets recommendations for a given bundle, bundleId of 0 returns randomized bundles - Accepts both pu |

### `GET` `/v1/bundles/{bundleId}/details`

**Parameters:**

- `bundleId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: Invalid bundle

### `GET` `/v1/bundles/{bundleId}/recommendations`

**Parameters:**

- `bundleId` (path, integer (required)) - 
- `numItems` (query, integer) - The number of recommended items to return.

**Responses:**

- `200` - OK
- `400` - 1: Invalid bundle 2: Error retrieving bundles 3: Error getting bundle recommendations 4: NumItems

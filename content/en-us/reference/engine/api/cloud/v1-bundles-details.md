---
title: V1 / Bundles / Details
type: cloud-api
tags: [Assets, Avatars]
---

# V1 / Bundles / Details

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/bundles/details` | Returns details about the given bundleIds. |

### `GET` `/v1/bundles/details`

**Parameters:**

- `bundleIds` (query, array (required)) - 

**Responses:**

- `200` - OK
- `400` - 3: Cannot request so many bundles at once.

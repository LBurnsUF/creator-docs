---
title: V2 / Inventory / Asset
type: cloud-api
tags: [Assets, Inventories]
---

# V2 / Inventory / Asset

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `DELETE` | `/v2/inventory/asset/{assetId}` | Give up an asset owned by the authenticated user. Assets that are created by Roblox user or are lim |

### `DELETE` `/v2/inventory/asset/{assetId}`

**Parameters:**

- `assetId` (path, integer (required)) - ID of the asset to delete.

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request. 4: You are not authorized.
- `403` - 0: Token Validation Failed 2: You don't own the specified item. 3: The item is not allowed to be d
- `404` - 1: The item does not exist.
- `500` - 0: An unknown error occured.

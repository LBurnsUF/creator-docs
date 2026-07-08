---
title: V2 / Assets
type: cloud-api
tags: [Assets, Inventories, Users]
---

# V2 / Assets

Cloud API resource group with 3 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/assets/{assetId}/bundles` | Lists bundles that contain the given asset (hydrated search-detail shape for marketplace). |
| `GET` | `/v2/assets/{assetId}/owners` | Gets a list of owners of an asset. |
| `GET` | `/v2/assets/{id}/versions` | Retrieves asset information for the specified asset ID. The authenticated user must be able to manag **DEPRECATED** |

### `GET` `/v2/assets/{assetId}/bundles`

**Parameters:**

- `assetId` (path, integer (required)) - Asset id.
- `Roblox-Place-Id` (header, integer (required)) - Roblox-Place-Id header.
- `Roblox-Game-Id` (header, string (required)) - Roblox-Game-Id header.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `400` - 1: Invalid assetId 4: Invalid Cursor.
- `403` - 7: User is unauthorized.

### `GET` `/v2/assets/{assetId}/owners`

**Parameters:**

- `assetId` (path, integer (required)) - The asset id.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - Sorted by userAssetId

**Responses:**

- `200` - OK
- `400` - 1: The asset id is invalid.
- `403` - 2: You do not have permission to view the owners of this asset.

### `GET` `/v2/assets/{id}/versions`

> **Deprecated**

Use OpenCloud Assets API instead.

**Parameters:**

- `id` (path, integer (required)) - The ID of the asset.Roblox.Platform.Assets.IAsset
- `Roblox-Place-Id` (header, integer (required)) - The ID of the place.Roblox.Platform.Assets.IPlace
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - Sort by version number, default is desc.

**Responses:**

- `200` - OK

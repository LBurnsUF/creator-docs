---
title: V1 / Assets
type: cloud-api
tags: [Assets, Avatars]
---

# V1 / Assets

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/assets/{assetId}/bundles` | Lists the bundles a particular asset belongs to. Use the Id of the last bundle in the response to ge |

### `GET` `/v1/assets/{assetId}/bundles`

**Parameters:**

- `assetId` (path, integer (required)) - 
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `400` - 1: Invalid assetId 4: Invalid Cursor.

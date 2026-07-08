---
title: V2 / Collectible Items
type: cloud-api
tags: [Assets, Inventories, Users]
---

# V2 / Collectible Items

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/collectible-items/{collectibleItemId}/owners` | Gets a list of owners of a collectible item. |

### `GET` `/v2/collectible-items/{collectibleItemId}/owners`

**Parameters:**

- `collectibleItemId` (path, string (required)) - The collectible item ID.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, integer) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `400` - 1: The collectible item id is invalid.
- `401` - 0: Authorization has been denied for this request.
- `403` - 2: You do not have permission to view the owners of this item.

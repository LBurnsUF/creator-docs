---
title: V1 / Creations / Get Assets
type: cloud-api
tags: [Assets]
---

# V1 / Creations / Get Assets

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/creations/get-assets` | Gets the user created asset information filtered by the given asset type. |

### `GET` `/v1/creations/get-assets`

**Parameters:**

- `assetType` (query, string (required)) - 
- `isArchived` (query, boolean) - 
- `groupId` (query, integer) - 
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.

**Responses:**

- `200` - OK
- `400` - 5: Invalid assetType 10: Invalid Asset Category
- `401` - 0: Authorization has been denied for this request.
- `403` - 7: User does not have necessary permissions for group 8: Asset type does not have necessary permiss
- `429` - 9: Flood Limit Exceeded
- `503` - 6: Service Unavailable

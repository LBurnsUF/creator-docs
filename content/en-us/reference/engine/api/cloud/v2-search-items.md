---
title: V2 / Search / Items
type: cloud-api
tags: [Assets, Avatars]
---

# V2 / Search / Items

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/search/items/details` | Search for catalog items. |

### `GET` `/v2/search/items/details`

This endpoint is for search by item type ids.

**Parameters:**

- `Taxonomy` (query, string) - 
- `AssetTypeIds` (query, array) - 
- `BundleTypeIds` (query, array) - 
- `CategoryFilter` (query, integer) - 
- `SortAggregation` (query, integer) - 
- `SortType` (query, integer) - 
- `CreatorType` (query, integer) - 
- `CreatorTargetId` (query, integer) - 
- `CreatorName` (query, string) - 
- `MaxPrice` (query, integer) - 
- `MinPrice` (query, integer) - 
- `Keyword` (query, string) - 
- `IncludeNotForSale` (query, boolean) - 
- `TriggeredByTopicDiscovery` (query, boolean) - 
- `SalesTypeFilter` (query, integer) - 
- `Topics` (query, string) - The input topics format is split by ",". E.g "topics=cat,hat,red".
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `400` - 1: Category subcategory selection not supported. 2: Creator id not found. 3: Creator type not foun
- `403` - 7: User is unauthorized. 22: In-experience search is denied for this place or universe.
- `429` - 8: The flood limit has been exceeded. 8: The flood limit has been exceeded.
- `503` - 18: Search request timed out

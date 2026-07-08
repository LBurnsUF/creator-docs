---
title: V1 / Games / Recommendations
type: cloud-api
tags: [Universes]
---

# V1 / Games / Recommendations

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/games/recommendations/game/{universeId}` | Get games recommendations based on a given universe |

### `GET` `/v1/games/recommendations/game/{universeId}`

**Parameters:**

- `universeId` (path, integer (required)) - The universe to base recommendations on
- `PaginationKey` (query, string (required)) - The key of a page, which includes the start row index and all other necessary information to query the data. This parameter is usually not needed for
- `MaxRows` (query, integer (required)) - The requested number of rows.
- `IsTruncatedResultsEnabled` (query, boolean (required)) - Truncated Results

**Responses:**

- `200` - OK
- `400` - 1: The pagination key is invalid.
- `404` - 2: The requested universe does not exist.

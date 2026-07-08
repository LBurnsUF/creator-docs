---
title: Legacy Localization Tables / V1 / Localization Table
type: cloud-api
tags: [Assets, Localization, Metadata]
---

# Legacy Localization Tables / V1 / Localization Table

Cloud API resource group with 7 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/legacy-localization-tables/v1/localization-table/limits` | Get limits for translation table entries operations |
| `GET` | `/legacy-localization-tables/v1/localization-table/tables/{assetId}` | Get table information by the assetId of the table. |
| `GET` | `/legacy-localization-tables/v1/localization-table/tables/{tableId}` | Get table information by the id of the table. |
| `PATCH` | `/legacy-localization-tables/v1/localization-table/tables/{tableId}` | Updates the tables contents based on what is provided. |
| `GET` | `/legacy-localization-tables/v1/localization-table/tables/{tableId}/entries` | Gets a batch of entries for a table. |
| `POST` | `/legacy-localization-tables/v1/localization-table/tables/{tableId}/entries/translation-history` | Gets the translation history for each entry passed in. |
| `GET` | `/legacy-localization-tables/v1/localization-table/tables/{tableId}/entry-count` | Gets the number of entries in the specified table |

### `GET` `/legacy-localization-tables/v1/localization-table/limits`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

### `GET` `/legacy-localization-tables/v1/localization-table/tables/{assetId}`

**Parameters:**

- `assetId` (path, integer (required)) - The asset id associated with the table.

**Responses:**

- `200` - OK
- `400` - 12: Invalid asset id.
- `401` - 0: Authorization has been denied for this request.
- `403` - 2: You do not have permission to get this table.

### `GET` `/legacy-localization-tables/v1/localization-table/tables/{tableId}`

**Parameters:**

- `tableId` (path, string (required)) - 

**Responses:**

- `200` - OK
- `400` - 3: Invalid table id.
- `401` - 0: Authorization has been denied for this request.
- `403` - 2: You do not have permission to get this table.

### `PATCH` `/legacy-localization-tables/v1/localization-table/tables/{tableId}`

**Parameters:**

- `tableId` (path, string (required)) - The table guid for the table to update.
- `gameId` (query, integer) - The game id.

**Request Body:** The metadata object is optional.

**Responses:**

- `200` - OK
- `400` - 3: Invalid table id. 4: Table does not exist. 10: Maximum entries exceeded. Please keep the number
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 6: You do not have permission to create this table.
- `503` - 17: Feature is disabled

### `GET` `/legacy-localization-tables/v1/localization-table/tables/{tableId}/entries`

**Parameters:**

- `tableId` (path, string (required)) - 
- `cursor` (query, string) - If null, there are no more entries in the table and you've reached the last page.
- `gameId` (query, integer) - 
- `entryFormat` (query, string) - 

**Responses:**

- `200` - OK
- `400` - 3: Invalid table id. 14: Invalid game id
- `401` - 0: Authorization has been denied for this request.
- `403` - 2: You do not have permission to get this table.

### `POST` `/legacy-localization-tables/v1/localization-table/tables/{tableId}/entries/translation-history`

**Parameters:**

- `tableId` (path, string (required)) - The entries' tableId.
- `gameId` (query, integer) - The game id.

**Request Body:** A request body containing all relevant data for entry history lookup.

**Responses:**

- `200` - OK
- `400` - 3: Invalid table id. 13: Request body can't be null 14: Invalid game id 16: Entries can't be null
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: You do not have permission to get this table.
- `429` - 24: Too many attempts.Please try again later.
- `503` - 17: Feature is disabled

### `GET` `/legacy-localization-tables/v1/localization-table/tables/{tableId}/entry-count`

**Parameters:**

- `tableId` (path, string (required)) - The table id
- `gameId` (query, integer) - The game id
- `entryFormat` (query, string) - 

**Responses:**

- `200` - OK
- `400` - 3: Invalid table id. 14: Invalid game id
- `401` - 0: Authorization has been denied for this request.
- `403` - 2: You do not have permission to get this table.

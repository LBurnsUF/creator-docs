---
title: V1 / Localization Table / Tables
type: cloud-api
tags: [Assets, Localization]
---

# V1 / Localization Table / Tables

Cloud API resource group with 8 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/localization-table/tables` | Creates a Localization Table with the given data. Note that this endpoint simply creates a table an |
| `GET` | `/v1/localization-table/tables/{assetId}` | Get table information by the assetId of the table. |
| `GET` | `/v1/localization-table/tables/{tableId}` | Get table information by the id of the table. |
| `PATCH` | `/v1/localization-table/tables/{tableId}` | Updates the tables contents based on what is provided. |
| `GET` | `/v1/localization-table/tables/{tableId}/entries` | Gets a batch of entries for a table. |
| `POST` | `/v1/localization-table/tables/{tableId}/entries/translation-feedback` | Gets the translation feedback for each entry passed in. |
| `POST` | `/v1/localization-table/tables/{tableId}/entries/translation-history` | Gets the translation history for each entry passed in. |
| `GET` | `/v1/localization-table/tables/{tableId}/entry-count` | Gets the number of entries in the specified table |

### `POST` `/v1/localization-table/tables`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: You do not have permission to get this table.

### `GET` `/v1/localization-table/tables/{assetId}`

**Parameters:**

- `assetId` (path, integer (required)) - The asset id associated with the table.

**Responses:**

- `200` - OK
- `400` - 12: Invalid asset id.
- `401` - 0: Authorization has been denied for this request.
- `403` - 2: You do not have permission to get this table.

### `GET` `/v1/localization-table/tables/{tableId}`

**Parameters:**

- `tableId` (path, string (required)) - 

**Responses:**

- `200` - OK
- `400` - 3: Invalid table id.
- `401` - 0: Authorization has been denied for this request.
- `403` - 2: You do not have permission to get this table.

### `PATCH` `/v1/localization-table/tables/{tableId}`

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

### `GET` `/v1/localization-table/tables/{tableId}/entries`

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

### `POST` `/v1/localization-table/tables/{tableId}/entries/translation-feedback`

**Parameters:**

- `tableId` (path, string (required)) - The entries' tableId.
- `gameId` (query, integer) - The game id.

**Request Body:** A request body containing all relevant data for entry translation feedback lookup.

**Responses:**

- `200` - OK
- `400` - 3: Invalid table id. 13: Request body can't be null 14: Invalid game id 16: Entries can't be null
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: You do not have permission to get this table.
- `429` - 24: Too many attempts.Please try again later.
- `503` - 17: Feature is disabled

### `POST` `/v1/localization-table/tables/{tableId}/entries/translation-history`

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

### `GET` `/v1/localization-table/tables/{tableId}/entry-count`

**Parameters:**

- `tableId` (path, string (required)) - The table id
- `gameId` (query, integer) - The game id
- `entryFormat` (query, string) - 

**Responses:**

- `200` - OK
- `400` - 3: Invalid table id. 14: Invalid game id
- `401` - 0: Authorization has been denied for this request.
- `403` - 2: You do not have permission to get this table.

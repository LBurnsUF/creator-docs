---
title: Toolbox Service / V1 / Saves
type: cloud-api
tags: [Creator Store]
---

# Toolbox Service / V1 / Saves

Cloud API resource group with 3 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `DELETE` | `/toolbox-service/v1/saves` | Deletes a save. [BETA] |
| `GET` | `/toolbox-service/v1/saves` | Gets saves from a collection. [BETA] |
| `POST` | `/toolbox-service/v1/saves` | Creates a save. [BETA] |

### `DELETE` `/toolbox-service/v1/saves`

**Operation:** `Saves_DeleteSave`

**Stability:** BETA

**Parameters:**

- `targetType` (query) - The type of asset being deleted
- `targetId` (query, integer) - The ID of the asset being deleted
- `collectionName` (query, string) - Custom collections are not currently supported. This field should be omitted.

**Responses:**

- `204` - No Content
- `400` - Bad Request
- `404` - Not Found

### `GET` `/toolbox-service/v1/saves`

**Operation:** `Saves_GetSaves`

**Stability:** BETA

**Parameters:**

- `targetType` (query) - The asset type to filter by
- `targetId` (query, integer) - The ID of the asset to filter by. If provided, targetType must also be provided.
- `collectionName` (query, string) - Custom collections are not currently supported. This field should be omitted.
- `sortBy` (query) - The field to sort by
- `sortDirection` (query) - The direction to sort by
- `limit` (query, integer) - The maximum number of saves to return
- `page` (query, integer) - The page number to return, starting from 1
- `keyword` (query, string) - The keyword to filter by
- `hideOwnedAssets` (query, boolean) - Whether to hide owned assets

**Responses:**

- `200` - Success
- `400` - Bad Request

### `POST` `/toolbox-service/v1/saves`

**Operation:** `Saves_CreateSave`

**Stability:** BETA

**Responses:**

- `201` - Created
- `400` - Bad Request
- `404` - Not Found
- `409` - Conflict

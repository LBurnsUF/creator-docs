---
title: Place Version History Api / V1
type: cloud-api
tags: [Places]
---

# Place Version History Api / V1

Cloud API resource group with 3 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/place-version-history-api/v1/{placeId}/contributors` | Endpoint used to fetch all previous contributors of a place. [EXPERIMENTAL] |
| `GET` | `/place-version-history-api/v1/{placeId}/history` | Endpoint used to get place versions, using various filters [EXPERIMENTAL] |
| `POST` | `/place-version-history-api/v1/{placeId}/version/{version}/notes` | Endpoint used to modify the notes of a particular version for a place. [EXPERIMENTAL] |

### `GET` `/place-version-history-api/v1/{placeId}/contributors`

**Operation:** `PlaceVersion_GetPlaceContributors`

**Stability:** EXPERIMENTAL

**Parameters:**

- `placeId` (path, integer (required)) - 
- `cursor` (query, string) - 
- `pageSize` (query, integer) - 

**Responses:**

- `200` - Success
- `400` - Bad Request
- `401` - Unauthorized
- `403` - Forbidden
- `500` - Server Error

### `GET` `/place-version-history-api/v1/{placeId}/history`

**Operation:** `PlaceVersion_GetPlaceVersionHistory`

**Stability:** EXPERIMENTAL

**Parameters:**

- `placeId` (path, integer (required)) - 
- `cursor` (query, string) - 
- `isPublished` (query, boolean) - 
- `hasNotes` (query, boolean) - 
- `saveType` (query, integer) - 
- `searchTerm` (query, string) - 
- `contributor` (query, integer) - 
- `startTime` (query, string) - 
- `endTime` (query, string) - 
- `pageSize` (query, integer) - 

**Responses:**

- `200` - Success
- `400` - Bad Request
- `401` - Unauthorized
- `403` - Forbidden
- `500` - Server Error

### `POST` `/place-version-history-api/v1/{placeId}/version/{version}/notes`

**Operation:** `PlaceVersion_UpdatePlaceVersionNotes`

**Stability:** EXPERIMENTAL

**Parameters:**

- `placeId` (path, integer (required)) - 
- `version` (path, string (required)) - 

**Responses:**

- `200` - Success
- `400` - Bad Request
- `401` - Unauthorized
- `403` - Forbidden
- `500` - Server Error

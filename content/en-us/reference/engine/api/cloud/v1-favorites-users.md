---
title: V1 / Favorites / Users
type: cloud-api
tags: [Assets, Avatars, Interactions, Users]
---

# V1 / Favorites / Users

Cloud API resource group with 8 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `DELETE` | `/v1/favorites/users/{userId}/assets/{assetId}/favorite` | Delete a favorite for an asset by the authenticated user. |
| `GET` | `/v1/favorites/users/{userId}/assets/{assetId}/favorite` | Gets the favorite model for the asset and user. |
| `POST` | `/v1/favorites/users/{userId}/assets/{assetId}/favorite` | Create a favorite for an asset by the authenticated user. |
| `DELETE` | `/v1/favorites/users/{userId}/bundles/{bundleId}/favorite` | Delete favorite for the bundle by the authenticated user. |
| `GET` | `/v1/favorites/users/{userId}/bundles/{bundleId}/favorite` | Gets the favorite model for the bundle and user. |
| `POST` | `/v1/favorites/users/{userId}/bundles/{bundleId}/favorite` | Create a favorite for the bundle by the authenticated user. |
| `GET` | `/v1/favorites/users/{userId}/favorites/{assetTypeId}/assets` | Lists the marketplace assets favorited by a given user with the given assetTypeId. |
| `GET` | `/v1/favorites/users/{userId}/favorites/{subtypeId}/bundles` | Lists the bundles favorited by a given user with the given bundle subtypeId.Switched to EAAS style p |

### `DELETE` `/v1/favorites/users/{userId}/assets/{assetId}/favorite`

**Parameters:**

- `userId` (path, integer (required)) - 
- `assetId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: Invalid user Id. 2: Invalid asset Id.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 6: You are not authorized to perform this action.
- `409` - 4: Asset is already not favorited.
- `429` - 5: This action was floodchecked. Please try again later.

### `GET` `/v1/favorites/users/{userId}/assets/{assetId}/favorite`

**Parameters:**

- `userId` (path, integer (required)) - 
- `assetId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: Invalid user Id. 2: Invalid asset Id.
- `401` - 0: Authorization has been denied for this request.

### `POST` `/v1/favorites/users/{userId}/assets/{assetId}/favorite`

**Parameters:**

- `userId` (path, integer (required)) - 
- `assetId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: Invalid user Id. 2: Invalid asset Id.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 6: You are not authorized to perform this action.
- `409` - 3: Asset is already favorited.
- `429` - 5: This action was floodchecked. Please try again later.

### `DELETE` `/v1/favorites/users/{userId}/bundles/{bundleId}/favorite`

**Parameters:**

- `userId` (path, integer (required)) - 
- `bundleId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: Invalid user Id. 2: Invalid bundle Id.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 6: You are not authorized to perform this action.
- `409` - 4: Bundle is already not favorited.
- `429` - 5: This action was floodchecked. Please try again later.

### `GET` `/v1/favorites/users/{userId}/bundles/{bundleId}/favorite`

**Parameters:**

- `userId` (path, integer (required)) - 
- `bundleId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: Invalid user Id. 2: Invalid bundle Id.
- `401` - 0: Authorization has been denied for this request.

### `POST` `/v1/favorites/users/{userId}/bundles/{bundleId}/favorite`

**Parameters:**

- `userId` (path, integer (required)) - 
- `bundleId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: Invalid user Id. 2: Invalid bundle Id.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 6: You are not authorized to perform this action.
- `409` - 3: Bundle is already favorited.
- `429` - 5: This action was floodchecked. Please try again later.

### `GET` `/v1/favorites/users/{userId}/favorites/{assetTypeId}/assets`

**Parameters:**

- `userId` (path, integer (required)) - 
- `assetTypeId` (path, integer (required)) - 
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `400` - 1: Invalid user Id. 8: Ascending order is not allowed. 11: Invalid asset type id.
- `500` - 99: Internal server error.

### `GET` `/v1/favorites/users/{userId}/favorites/{subtypeId}/bundles`

**Parameters:**

- `userId` (path, integer (required)) - 
- `subtypeId` (path, integer (required)) - 
- `itemsPerPage` (query, integer) - 
- `cursor` (query, string) - 
- `isPrevious` (query, boolean) - 

**Responses:**

- `200` - OK
- `400` - 1: Invalid user Id. 3: Cannot request so many bundles at once. 10: Invalid previous pagination req
- `401` - 0: Authorization has been denied for this request.
- `403` - 6: You are not authorized to perform this action.
- `500` - 11: Internal server error. Please check if you have provided correct pagination cursor

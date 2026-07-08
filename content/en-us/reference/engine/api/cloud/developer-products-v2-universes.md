---
title: Developer Products / V2 / Universes
type: cloud-api
tags: [Developer products]
---

# Developer Products / V2 / Universes

Cloud API resource group with 4 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/developer-products/v2/universes/{universeId}/developer-products` | Create developer product [BETA] |
| `GET` | `/developer-products/v2/universes/{universeId}/developer-products/creator` | List developer products by universe with configuration details [BETA] |
| `PATCH` | `/developer-products/v2/universes/{universeId}/developer-products/{productId}` | Update developer product [BETA] |
| `GET` | `/developer-products/v2/universes/{universeId}/developer-products/{productId}/creator` | Get developer product with configuration details [BETA] |

### `POST` `/developer-products/v2/universes/{universeId}/developer-products`

**Operation:** `DeveloperProducts_CreateDeveloperProductV2`

**Stability:** BETA

Creates a new developer product with the provided configuration details.

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID.

**Responses:**

- `200` - Success
- `400` - Bad Request
- `401` - Unauthorized
- `403` - Forbidden
- `404` - Not Found

### `GET` `/developer-products/v2/universes/{universeId}/developer-products/creator`

**Operation:** `DeveloperProducts_ListDeveloperProductConfigsByUniverseV2`

**Stability:** BETA

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID.
- `pageSize` (query, integer) - The number of results to return. Defaults to 50.
- `pageToken` (query, string) - The cursor token for pagination.

**Responses:**

- `200` - Success
- `400` - Bad Request
- `401` - Unauthorized
- `403` - Forbidden
- `404` - Not Found

### `PATCH` `/developer-products/v2/universes/{universeId}/developer-products/{productId}`

**Operation:** `DeveloperProducts_UpdateDeveloperProductV2`

**Stability:** BETA

Updates a developer product with the provided configuration details. 
Note that only fields provided in the request will be updated.

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID.
- `productId` (path, integer (required)) - The product ID of the developer product.

**Responses:**

- `204` - No Content
- `400` - Bad Request
- `401` - Unauthorized
- `403` - Forbidden
- `404` - Not Found
- `409` - Conflict

### `GET` `/developer-products/v2/universes/{universeId}/developer-products/{productId}/creator`

**Operation:** `DeveloperProducts_GetDeveloperProductConfigV2`

**Stability:** BETA

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID.
- `productId` (path, integer (required)) - The product ID of the developer product.

**Responses:**

- `200` - Success
- `401` - Unauthorized
- `403` - Forbidden
- `404` - Not Found

---
title: V2 / Places
type: cloud-api
tags: [Places]
---

# V2 / Places

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/places/{placeId}` | Gets the place configuration for the place with the id placeId |
| `PATCH` | `/v2/places/{placeId}` | Updates the place configuration for the place with the id placeId |

### `GET` `/v2/places/{placeId}`

**Parameters:**

- `placeId` (path, integer (required)) - The place id for the place to be updated.

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - Authenticated user is not authorized to manage this place.
- `404` - placeId Place not found.

### `PATCH` `/v2/places/{placeId}`

**Parameters:**

- `placeId` (path, integer (required)) - The place id for the place to be updated.

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - Authenticated user is not authorized to manage this place. 0: Token Validation Failed
- `404` - placeId Place not found.

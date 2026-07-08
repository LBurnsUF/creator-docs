---
title: Legacy Develop / V1 / Universes
type: cloud-api
tags: [Team Create, Universes]
---

# Legacy Develop / V1 / Universes

Cloud API resource group with 8 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/legacy-develop/v1/universes/multiget/permissions` | Returns an array of granted and declined permissions related to the universes with the ids in ids fo |
| `GET` | `/legacy-develop/v1/universes/multiget/teamcreate` | Gets TeamCreate settings for multiple universes specified by Ids |
| `POST` | `/legacy-develop/v1/universes/{universeId}/activate` | Activates a universes. |
| `POST` | `/legacy-develop/v1/universes/{universeId}/deactivate` | Deactivates a universe. |
| `GET` | `/legacy-develop/v1/universes/{universeId}/permissions` | Returns list of granted and declined permissions related to the universe with the id universeId for  |
| `GET` | `/legacy-develop/v1/universes/{universeId}/teamcreate` | Gets TeamCreate settings for an Roblox.Platform.Universes.IUniverse. |
| `PATCH` | `/legacy-develop/v1/universes/{universeId}/teamcreate` | Edit team create settings for a universe. |
| `DELETE` | `/legacy-develop/v1/universes/{universeId}/teamcreate/memberships` | Removes a user from a TeamCreate permissions list. |

### `GET` `/legacy-develop/v1/universes/multiget/permissions`

If a universe can not be found for a given ID (such as -1) it will be skipped.

**Parameters:**

- `ids` (query, array (required)) - The universe ids.

**Responses:**

- `200` - OK
- `400` - 8: No universe IDs sent to get. 9: Too many universe IDs sent to get, the limit is: 
- `401` - 0: Authorization has been denied for this request.

### `GET` `/legacy-develop/v1/universes/multiget/teamcreate`

**Parameters:**

- `ids` (query, array (required)) - The universe Ids.

**Responses:**

- `200` - OK
- `400` - Roblox.Api.Develop.ResponseEnums.TeamCreateErrors.TooManyUniverseIdsSent
- `401` - 0: Authorization has been denied for this request.

### `POST` `/legacy-develop/v1/universes/{universeId}/activate`

**Parameters:**

- `universeId` (path, integer (required)) - The universe id.

**Responses:**

- `200` - OK
- `400` - 1: The universe does not exist. 2: This universe does not have a root place.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 3: You are not authorized to configure this universe. 6: The root place

### `POST` `/legacy-develop/v1/universes/{universeId}/deactivate`

**Parameters:**

- `universeId` (path, integer (required)) - The universe id.

**Responses:**

- `200` - OK
- `400` - 1: The universe does not exist. 2: This universe does not have a root place.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 3: You are not authorized to configure this universe.

### `GET` `/legacy-develop/v1/universes/{universeId}/permissions`

**Parameters:**

- `universeId` (path, integer (required)) - The universe id.

**Responses:**

- `200` - OK
- `400` - 1: The universe does not exist.
- `401` - 0: Authorization has been denied for this request.

### `GET` `/legacy-develop/v1/universes/{universeId}/teamcreate`

**Parameters:**

- `universeId` (path, integer (required)) - The universe Id.

**Responses:**

- `200` - OK
- `400` - Roblox.Api.Develop.ResponseEnums.TeamCreateErrors.InvalidUniverse
- `401` - 0: Authorization has been denied for this request.
- `403` - Roblox.Api.Develop.ResponseEnums.TeamCreateErrors.Unauthorized

### `PATCH` `/legacy-develop/v1/universes/{universeId}/teamcreate`

Enables, or disables team create for a universe.

**Parameters:**

- `universeId` (path, integer (required)) - The universe Id.

**Responses:**

- `200` - OK
- `400` - Roblox.Api.Develop.ResponseEnums.TeamCreateErrors.InvalidUniverse
- `401` - 0: Authorization has been denied for this request.
- `403` - Roblox.Api.Develop.ResponseEnums.TeamCreateErrors.Unauthorized 0: Token Validation Failed

### `DELETE` `/legacy-develop/v1/universes/{universeId}/teamcreate/memberships`

**Parameters:**

- `universeId` (path, integer (required)) - The universe Id.

**Responses:**

- `200` - OK
- `400` - Roblox.Api.Develop.ResponseEnums.TeamCreateErrors.InvalidUniverse OR Roblox.Api.Develop.ResponseEnum
- `401` - 0: Authorization has been denied for this request.
- `403` - Roblox.Api.Develop.ResponseEnums.TeamCreateErrors.TeamCreateDisabled 0: Token Validation Failed

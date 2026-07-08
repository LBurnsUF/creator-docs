---
title: V1 / Universes
type: cloud-api
tags: [Badges, Places, Private servers, Team Create, Universes]
---

# V1 / Universes

Cloud API resource group with 16 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/universes/{universeId}` | Gets a Roblox.Api.Develop.Models.UniverseModel. |
| `POST` | `/v1/universes/{universeId}/activate` | Activates a universes. |
| `GET` | `/v1/universes/{universeId}/activation-eligibility` | Returns the result of various checks for a user's eligibility to activate a given universe from priv |
| `GET` | `/v1/universes/{universeId}/badges` | Gets badges by their awarding game. |
| `POST` | `/v1/universes/{universeId}/badges` | Creates a new badge. |
| `GET` | `/v1/universes/{universeId}/configuration` | Get settings for an owned universe. |
| `PATCH` | `/v1/universes/{universeId}/configuration` | Update universe settings for an owned universe. |
| `GET` | `/v1/universes/{universeId}/configuration/vip-servers` | Get settings for an owned universe's VIP servers. |
| `POST` | `/v1/universes/{universeId}/deactivate` | Deactivates a universe. |
| `GET` | `/v1/universes/{universeId}/free-badges-quota` | Gets the number of free badges left for the current UTC day by their awarding game. |
| `GET` | `/v1/universes/{universeId}/permissions` | Returns list of granted and declined permissions related to the universe with the id universeId for  |
| `GET` | `/v1/universes/{universeId}/places` | Gets a list of places for a universe. |
| `GET` | `/v1/universes/{universeId}/stats` | Get statistics data for a universe. |
| `GET` | `/v1/universes/{universeId}/teamcreate` | Gets TeamCreate settings for an Roblox.Platform.Universes.IUniverse. |
| `PATCH` | `/v1/universes/{universeId}/teamcreate` | Edit team create settings for a universe. |
| `DELETE` | `/v1/universes/{universeId}/teamcreate/memberships` | Removes a user from a TeamCreate permissions list. |

### `GET` `/v1/universes/{universeId}`

**Parameters:**

- `universeId` (path, integer (required)) - The Universe id.

**Responses:**

- `200` - OK
- `400` - 1: The universe does not exist.

### `POST` `/v1/universes/{universeId}/activate`

**Parameters:**

- `universeId` (path, integer (required)) - The universe id.

**Responses:**

- `200` - OK
- `400` - 1: The universe does not exist. 2: This universe does not have a root place.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 3: You are not authorized to configure this universe. 6: The root place

### `GET` `/v1/universes/{universeId}/activation-eligibility`

**Parameters:**

- `universeId` (path, integer (required)) - The universe id.

**Responses:**

- `200` - OK

### `GET` `/v1/universes/{universeId}/badges`

**Parameters:**

- `universeId` (path, integer (required)) - The universe Id.
- `sortBy` (query, string) - The key to sort badges by.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `400` - 26: The pagination cursor is invalid or incompatible with the current request.
- `404` - 3: The game is invalid or does not exist.

### `POST` `/v1/universes/{universeId}/badges`

**Parameters:**

- `universeId` (path, integer (required)) - The ID of the universe to create the badge for.

**Responses:**

- `200` - OK
- `400` - 11: The badge icon is invalid. 14: Invalid badge name. 15: Invalid badge description. 16: Payment
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 6: Text moderated. 12: You do not have permission to manage this game's
- `404` - 3: The game is invalid or does not exist.
- `429` - 13: Too many requests, try again later.

### `GET` `/v1/universes/{universeId}/configuration`

**Parameters:**

- `universeId` (path, integer (required)) - The universe Id.

**Responses:**

- `200` - OK
- `400` - 1: The universe does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 2: You are not authorized to configure this universe.

### `PATCH` `/v1/universes/{universeId}/configuration`

**Parameters:**

- `universeId` (path, integer (required)) - The universeId.

**Request Body:** The Roblox.Api.Develop.Models.UniverseSettingsRequest model.

**Responses:**

- `200` - OK
- `400` - 1: The universe does not exist. 3: Invalid UniverseAvatarType. 4: Invalid UniverseScaleType. 5: I
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: You are not authorized to configure this universe. 14: You are not a
- `409` - 9: Failed to shutdown all intances of game after changing AvatarType. The change has been reverted.

### `GET` `/v1/universes/{universeId}/configuration/vip-servers`

**Parameters:**

- `universeId` (path, integer (required)) - The universe Id.

**Responses:**

- `200` - OK
- `400` - 1: The universe does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 2: You are not authorized to configure this universe.

### `POST` `/v1/universes/{universeId}/deactivate`

**Parameters:**

- `universeId` (path, integer (required)) - The universe id.

**Responses:**

- `200` - OK
- `400` - 1: The universe does not exist. 2: This universe does not have a root place.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 3: You are not authorized to configure this universe.

### `GET` `/v1/universes/{universeId}/free-badges-quota`

**Parameters:**

- `universeId` (path, integer (required)) - The universe Id.

**Responses:**

- `200` - OK
- `404` - 3: The game is invalid or does not exist.

### `GET` `/v1/universes/{universeId}/permissions`

**Parameters:**

- `universeId` (path, integer (required)) - The universe id.

**Responses:**

- `200` - OK
- `400` - 1: The universe does not exist.
- `401` - 0: Authorization has been denied for this request.

### `GET` `/v1/universes/{universeId}/places`

**Parameters:**

- `universeId` (path, integer (required)) - The asset id.
- `isUniverseCreation` (query, boolean) - 
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - Sorted by placeId

**Responses:**

- `200` - OK

### `GET` `/v1/universes/{universeId}/stats`

**Parameters:**

- `universeId` (path, integer (required)) - The universe id.
- `Type` (query, string (required)) - 
- `StartTime` (query, string (required)) - 
- `EndTime` (query, string (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: The Universe is invalid. 3: Too many data points requested. 4: The requested data type is not k
- `401` - 0: Authorization has been denied for this request. 2: Not authorized to perform this action.

### `GET` `/v1/universes/{universeId}/teamcreate`

**Parameters:**

- `universeId` (path, integer (required)) - The universe Id.

**Responses:**

- `200` - OK
- `400` - Roblox.Api.Develop.ResponseEnums.TeamCreateErrors.InvalidUniverse
- `401` - 0: Authorization has been denied for this request.
- `403` - Roblox.Api.Develop.ResponseEnums.TeamCreateErrors.Unauthorized

### `PATCH` `/v1/universes/{universeId}/teamcreate`

Enables, or disables team create for a universe.

**Parameters:**

- `universeId` (path, integer (required)) - The universe Id.

**Responses:**

- `200` - OK
- `400` - Roblox.Api.Develop.ResponseEnums.TeamCreateErrors.InvalidUniverse
- `401` - 0: Authorization has been denied for this request.
- `403` - Roblox.Api.Develop.ResponseEnums.TeamCreateErrors.Unauthorized 0: Token Validation Failed

### `DELETE` `/v1/universes/{universeId}/teamcreate/memberships`

**Parameters:**

- `universeId` (path, integer (required)) - The universe Id.

**Responses:**

- `200` - OK
- `400` - Roblox.Api.Develop.ResponseEnums.TeamCreateErrors.InvalidUniverse OR Roblox.Api.Develop.ResponseEnum
- `401` - 0: Authorization has been denied for this request.
- `403` - Roblox.Api.Develop.ResponseEnums.TeamCreateErrors.TeamCreateDisabled 0: Token Validation Failed

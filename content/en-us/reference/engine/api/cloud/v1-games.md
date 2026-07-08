---
title: V1 / Games
type: cloud-api
tags: [Assets, Interactions, Private servers, Thumbnails, Universes]
---

# V1 / Games

Cloud API resource group with 11 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/games` | Gets a list of games' detail |
| `POST` | `/v1/games/{gameId}/thumbnail/image` | Uploads a game thumbnail. |
| `GET` | `/v1/games/{placeId}/private-servers` |  |
| `GET` | `/v1/games/{universeId}/favorites` | Returns if a game was marked as favorite for the authenticated user |
| `POST` | `/v1/games/{universeId}/favorites` | Favors (or unfavors) a game for the authenticated user |
| `GET` | `/v1/games/{universeId}/favorites/count` | Get the favorites count of a specific game. |
| `GET` | `/v1/games/{universeId}/media` | Get the game media data **DEPRECATED** |
| `GET` | `/v1/games/{universeId}/thumbnails` | Fetches game thumbnail URLs for a list of universes' thumbnail ids. Ids that do not correspond to a  [STABLE] |
| `PATCH` | `/v1/games/{universeId}/user-votes` |  |
| `GET` | `/v1/games/{universeId}/votes` |  |
| `GET` | `/v1/games/{universeId}/votes/user` |  |

### `GET` `/v1/games`

**Parameters:**

- `universeIds` (query, array (required)) - A list of universe Ids. Cannot exceed a maximum of 50 IDs.
- `fields` (query, string) - Optional comma-separated list of field names to include in the response. When omitted, all fields are returned.

**Responses:**

- `200` - OK
- `400` - 8: The universe IDs specified are invalid. 9: Too many universe IDs were requested.
- `429` - 4: Too many requests have been made.

### `POST` `/v1/games/{gameId}/thumbnail/image`

**Parameters:**

- `gameId` (path, integer (required)) - The universe Id.

**Responses:**

- `200` - OK
- `400` - 1: File uploaded does not match known image format. Try converting to png. 2: File not present in r
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 5: You do not have permission to manage this item.
- `404` - 4: Target item is invalid or does not exist.
- `429` - 3: You're uploading too much, please wait and try again later.

### `GET` `/v1/games/{placeId}/private-servers`

**Operation:** `PrivateServers_GetPrivateServerList`

**Parameters:**

- `placeId` (path, integer (required)) - 
- `exclusiveStartKeyCursor` (query) - 
- `excludeFriendServers` (query, boolean) - 

**Responses:**

- `200` - Success

### `GET` `/v1/games/{universeId}/favorites`

**Parameters:**

- `universeId` (path, integer (required)) - The Id of the universe.

**Responses:**

- `200` - OK
- `400` - 3: The universe's root place is invalid.
- `401` - 0: Authorization has been denied for this request.
- `404` - 2: The requested universe does not exist.

### `POST` `/v1/games/{universeId}/favorites`

**Parameters:**

- `universeId` (path, integer (required)) - The Id of the universe.

**Request Body:** Request data.

**Responses:**

- `200` - OK
- `400` - 3: The universe's root place is invalid.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 11: You are not authorized to perform this action.
- `404` - 2: The requested universe does not exist.
- `429` - 4: Too many requests have been made.

### `GET` `/v1/games/{universeId}/favorites/count`

**Parameters:**

- `universeId` (path, integer (required)) - The Id of the universe.

**Responses:**

- `200` - OK
- `400` - 3: The universe's root place is invalid.
- `404` - 2: The requested universe does not exist.

### `GET` `/v1/games/{universeId}/media`

> **Deprecated**

Use https://games.roblox.com/v2/games/{universeId}/media instead

**Parameters:**

- `universeId` (path, integer (required)) - The id of the universe we get media data from.

**Responses:**

- `200` - OK
- `400` - 3: The universe's root place is invalid.
- `404` - 2: The requested universe does not exist.

### `GET` `/v1/games/{universeId}/thumbnails`

**Stability:** STABLE

**Parameters:**

- `universeId` (path, integer (required)) - 
- `thumbnailIds` (query, array (required)) - 
- `size` (query, string) - The thumbnail size, formatted widthxheight
- `format` (query, string) - The thumbnail format
- `isCircular` (query, boolean) - The circle thumbnail output parameter, true or false

**Responses:**

- `200` - OK
- `400` - 1: There are too many requested Ids. 2: The requested image format is invalid. Please see documenta
- `404` - 5: The requested universe does not exist.

### `PATCH` `/v1/games/{universeId}/user-votes`

**Operation:** `Voting_VoteGame`

**Parameters:**

- `universeId` (path, integer (required)) - 

**Responses:**

- `200` - Success

### `GET` `/v1/games/{universeId}/votes`

**Operation:** `Voting_GetGameVoteStatus`

**Parameters:**

- `universeId` (path, integer (required)) - 

**Responses:**

- `200` - Success

### `GET` `/v1/games/{universeId}/votes/user`

**Operation:** `Voting_GetGameVoteStatusForUser`

**Parameters:**

- `universeId` (path, integer (required)) - 

**Responses:**

- `200` - Success

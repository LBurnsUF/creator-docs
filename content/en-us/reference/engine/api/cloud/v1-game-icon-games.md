---
title: V1 / Game Icon / Games
type: cloud-api
tags: [Localization, Universes]
---

# V1 / Game Icon / Games

Cloud API resource group with 3 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/game-icon/games/{gameId}` | Get all icons for a game |
| `DELETE` | `/v1/game-icon/games/{gameId}/language-codes/{languageCode}` | Delete a localized icon from a game |
| `POST` | `/v1/game-icon/games/{gameId}/language-codes/{languageCode}` | Update a game's icon |

### `GET` `/v1/game-icon/games/{gameId}`

**Parameters:**

- `gameId` (path, integer (required)) - The id of the game
- `width` (query, integer) - The width of the icon to request
- `height` (query, integer) - The height of the icon to request

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id 52: Image dimensions are invalid
- `401` - 0: Authorization has been denied for this request.
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

### `DELETE` `/v1/game-icon/games/{gameId}/language-codes/{languageCode}`

**Parameters:**

- `gameId` (path, integer (required)) - The id of the game
- `languageCode` (path, string (required)) - The language code of the localized icon to delete

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id 22: Invalid language code 23: You can't delete translations for source languag
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

### `POST` `/v1/game-icon/games/{gameId}/language-codes/{languageCode}`

**Parameters:**

- `gameId` (path, integer (required)) - The id of the game
- `languageCode` (path, string (required)) - The language code of this icon to update

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id 22: Invalid language code 26: You can't update translations for source languag
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `429` - 24: Too many attempts.Please try again later.
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

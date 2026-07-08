---
title: V1 / Name Description / Games
type: cloud-api
tags: [Localization, Universes]
---

# V1 / Name Description / Games

Cloud API resource group with 3 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/name-description/games/translation-history` | Gets the history for name or description in a provided language. |
| `GET` | `/v1/name-description/games/{gameId}` | Gets a game's name and description in all supported languages |
| `PATCH` | `/v1/name-description/games/{gameId}` | Updates a game's name and/or description in multiple languages. |

### `POST` `/v1/name-description/games/translation-history`

**Request Body:** The request.

**Responses:**

- `200` - OK
- `400` - 13: Request body can't be null 14: Invalid game id 18: You do not have permission to manage this g
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

### `GET` `/v1/name-description/games/{gameId}`

**Parameters:**

- `gameId` (path, integer (required)) - The id of the game

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id
- `503` - 17: Feature is disabled

### `PATCH` `/v1/name-description/games/{gameId}`

**Parameters:**

- `gameId` (path, integer (required)) - The id of the game.

**Request Body:** The request body.

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id 19: New name is null or whitespaces or new name/description is too long 20: Ne
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `503` - 17: Feature is disabled

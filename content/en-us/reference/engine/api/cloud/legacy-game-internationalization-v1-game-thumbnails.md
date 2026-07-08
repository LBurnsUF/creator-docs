---
title: Legacy Game Internationalization / V1 / Game Thumbnails
type: cloud-api
tags: [Localization, Thumbnails, Universes]
---

# Legacy Game Internationalization / V1 / Game Thumbnails

Cloud API resource group with 4 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/legacy-game-internationalization/v1/game-thumbnails/games/{gameId}/language-codes/{languageCode}/alt-text` | Updates the game thumbnail alt text. |
| `POST` | `/legacy-game-internationalization/v1/game-thumbnails/games/{gameId}/language-codes/{languageCode}/image` | Uploads the game thumbnail. |
| `POST` | `/legacy-game-internationalization/v1/game-thumbnails/games/{gameId}/language-codes/{languageCode}/images/order` | Orders the specified image Ids for the game thumbnails. |
| `DELETE` | `/legacy-game-internationalization/v1/game-thumbnails/games/{gameId}/language-codes/{languageCode}/images/{imageId}` | Deletes the game thumbnail. |

### `POST` `/legacy-game-internationalization/v1/game-thumbnails/games/{gameId}/language-codes/{languageCode}/alt-text`

**Parameters:**

- `gameId` (path, integer (required)) - The game identifier.
- `languageCode` (path, string (required)) - The language code.

**Request Body:** The game thumbnail alt text update request.

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id 19: New name is null or whitespaces or new name/description is too long 20: Ne
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `429` - 24: Too many attempts.Please try again later.
- `500` - 0: An unknown error occurred. 88: Failed to filter text
- `503` - 17: Feature is disabled

### `POST` `/legacy-game-internationalization/v1/game-thumbnails/games/{gameId}/language-codes/{languageCode}/image`

**Parameters:**

- `gameId` (path, integer (required)) - The game identifier.
- `languageCode` (path, string (required)) - The language code.

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id 22: Invalid language code 26: You can't update translations for source languag
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `429` - 24: Too many attempts.Please try again later.
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

### `POST` `/legacy-game-internationalization/v1/game-thumbnails/games/{gameId}/language-codes/{languageCode}/images/order`

**Parameters:**

- `gameId` (path, integer (required)) - The game identifier.
- `languageCode` (path, string (required)) - The language code.

**Request Body:** The request.

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id 22: Invalid language code 26: You can't update translations for source languag
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `503` - 17: Feature is disabled

### `DELETE` `/legacy-game-internationalization/v1/game-thumbnails/games/{gameId}/language-codes/{languageCode}/images/{imageId}`

**Parameters:**

- `gameId` (path, integer (required)) - The game identifier.
- `languageCode` (path, string (required)) - The language code.
- `imageId` (path, integer (required)) - The image identifier.

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id 22: Invalid language code 23: You can't delete translations for source languag
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `503` - 17: Feature is disabled

---
title: Legacy Game Internationalization / V1 / Game Passes
type: cloud-api
tags: [Game passes, Localization]
---

# Legacy Game Internationalization / V1 / Game Passes

Cloud API resource group with 8 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `PATCH` | `/legacy-game-internationalization/v1/game-passes/{gamePassId}/description/language-codes/{languageCode}` | Update localized description of a game pass |
| `GET` | `/legacy-game-internationalization/v1/game-passes/{gamePassId}/icons` | Get all icons for a game pass |
| `DELETE` | `/legacy-game-internationalization/v1/game-passes/{gamePassId}/icons/language-codes/{languageCode}` | Delete a localized icon from a game pass |
| `POST` | `/legacy-game-internationalization/v1/game-passes/{gamePassId}/icons/language-codes/{languageCode}` | Update a game pass's icon |
| `GET` | `/legacy-game-internationalization/v1/game-passes/{gamePassId}/name-description` | Get all names and descriptions of a game pass |
| `DELETE` | `/legacy-game-internationalization/v1/game-passes/{gamePassId}/name-description/language-codes/{languageCode}` | Delete localized name and description of a game pass |
| `PATCH` | `/legacy-game-internationalization/v1/game-passes/{gamePassId}/name-description/language-codes/{languageCode}` | Update localized name and description of a game pass |
| `PATCH` | `/legacy-game-internationalization/v1/game-passes/{gamePassId}/name/language-codes/{languageCode}` | Update localized name of a game pass |

### `PATCH` `/legacy-game-internationalization/v1/game-passes/{gamePassId}/description/language-codes/{languageCode}`

**Parameters:**

- `gamePassId` (path, integer (required)) - The game pass id
- `languageCode` (path, string (required)) - The language code of description to update

**Request Body:** The request

**Responses:**

- `200` - OK
- `400` - 13: Request body can't be null 19: New name is null or whitespaces or new name/description is too l
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `503` - 17: Feature is disabled

### `GET` `/legacy-game-internationalization/v1/game-passes/{gamePassId}/icons`

**Parameters:**

- `gamePassId` (path, integer (required)) - The game pass id
- `width` (query, integer) - The width of the icon to request
- `height` (query, integer) - The height of the icon to request

**Responses:**

- `200` - OK
- `400` - 52: Image dimensions are invalid 61: Invalid game pass id
- `401` - 0: Authorization has been denied for this request.
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

### `DELETE` `/legacy-game-internationalization/v1/game-passes/{gamePassId}/icons/language-codes/{languageCode}`

**Parameters:**

- `gamePassId` (path, integer (required)) - The game pass id
- `languageCode` (path, string (required)) - The language code of the localized icon to delete

**Responses:**

- `200` - OK
- `400` - 22: Invalid language code 23: You can't delete translations for source language 53: Language is no
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

### `POST` `/legacy-game-internationalization/v1/game-passes/{gamePassId}/icons/language-codes/{languageCode}`

**Parameters:**

- `gamePassId` (path, integer (required)) - The game pass id
- `languageCode` (path, string (required)) - The language code of this icon to update

**Responses:**

- `200` - OK
- `400` - 22: Invalid language code 26: You can't update translations for source language 45: File uploaded 
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `429` - 24: Too many attempts.Please try again later.
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

### `GET` `/legacy-game-internationalization/v1/game-passes/{gamePassId}/name-description`

**Parameters:**

- `gamePassId` (path, integer (required)) - The game pass Id

**Responses:**

- `200` - OK
- `400` - 61: Invalid game pass id
- `401` - 0: Authorization has been denied for this request.
- `503` - 17: Feature is disabled

### `DELETE` `/legacy-game-internationalization/v1/game-passes/{gamePassId}/name-description/language-codes/{languageCode}`

**Parameters:**

- `gamePassId` (path, integer (required)) - The game pass id
- `languageCode` (path, string (required)) - The language code of the name and description to delete

**Responses:**

- `200` - OK
- `400` - 22: Invalid language code 23: You can't delete translations for source language 53: Language is no
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `503` - 17: Feature is disabled

### `PATCH` `/legacy-game-internationalization/v1/game-passes/{gamePassId}/name-description/language-codes/{languageCode}`

**Parameters:**

- `gamePassId` (path, integer (required)) - The game pass id
- `languageCode` (path, string (required)) - The language code of the name/description to update

**Request Body:** The request

**Responses:**

- `200` - OK
- `400` - 13: Request body can't be null 19: New name is null or whitespaces or new name/description is too l
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `503` - 17: Feature is disabled

### `PATCH` `/legacy-game-internationalization/v1/game-passes/{gamePassId}/name/language-codes/{languageCode}`

**Parameters:**

- `gamePassId` (path, integer (required)) - The game pass id
- `languageCode` (path, string (required)) - The language code of the name to update

**Request Body:** The request

**Responses:**

- `200` - OK
- `400` - 13: Request body can't be null 19: New name is null or whitespaces or new name/description is too l
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `503` - 17: Feature is disabled

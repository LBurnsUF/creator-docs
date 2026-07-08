---
title: V1 / Supported Languages / Games
type: cloud-api
tags: [Localization, Universes]
---

# V1 / Supported Languages / Games

Cloud API resource group with 8 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/supported-languages/games/{gameId}` | Get the supported languages for a game. |
| `PATCH` | `/v1/supported-languages/games/{gameId}` | Add or remove supported languages for a game. |
| `GET` | `/v1/supported-languages/games/{gameId}/automatic-translation-status` | Get the automatic translation status of supported languages for a game. |
| `GET` | `/v1/supported-languages/games/{gameId}/in-experience-language-selection` | Get the user's in-experience language selector languages for a game. |
| `PATCH` | `/v1/supported-languages/games/{gameId}/languages/{languageCode}/automatic-translation-status` | Enable or disable automatic translation for a game and language. |
| `PATCH` | `/v1/supported-languages/games/{gameId}/languages/{languageCode}/image-translation-status` | Enable or disable image translation for a game and language. |
| `PATCH` | `/v1/supported-languages/games/{gameId}/languages/{languageCode}/universe-display-info-automatic-translation-settings` | Update the switch which controls if the UniverseDisplayInformation should be automatically translate |
| `GET` | `/v1/supported-languages/games/{gameId}/universe-display-info-automatic-translation-settings` | Get UniverseDisplayInfo automatic translation settings. |

### `GET` `/v1/supported-languages/games/{gameId}`

**Parameters:**

- `gameId` (path, integer (required)) - The id of the game.

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id
- `503` - 17: Feature is disabled

### `PATCH` `/v1/supported-languages/games/{gameId}`

**Parameters:**

- `gameId` (path, integer (required)) - The id of the game.

**Request Body:** The languages to add or remove. LanguageCodeType can be "Language" or "Locale".

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id 22: Invalid language code 49: Duplicate language codes are not allowed.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `503` - 17: Feature is disabled

### `GET` `/v1/supported-languages/games/{gameId}/automatic-translation-status`

**Parameters:**

- `gameId` (path, integer (required)) - The id of the game.

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id
- `401` - 0: Authorization has been denied for this request.
- `403` - 18: You do not have permission to manage this game
- `503` - 17: Feature is disabled

### `GET` `/v1/supported-languages/games/{gameId}/in-experience-language-selection`

**Parameters:**

- `gameId` (path, integer (required)) - The id of the game.

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id
- `503` - 17: Feature is disabled

### `PATCH` `/v1/supported-languages/games/{gameId}/languages/{languageCode}/automatic-translation-status`

**Parameters:**

- `gameId` (path, integer (required)) - The id of the game.
- `languageCode` (path, string (required)) - The language to enable or disable for automatic translation.

**Request Body:** Flag to indicate if automatic translation should be enabled or disabled.

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id 22: Invalid language code 53: Language is not supported for the game. 72: Aut
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `503` - 17: Feature is disabled

### `PATCH` `/v1/supported-languages/games/{gameId}/languages/{languageCode}/image-translation-status`

**Parameters:**

- `gameId` (path, integer (required)) - The id of the game.
- `languageCode` (path, string (required)) - The language to enable or disable for image translation.

**Request Body:** Flag to indicate if image translation should be enabled or disabled.

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id 22: Invalid language code 53: Language is not supported for the game. 93: Ima
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `503` - 17: Feature is disabled

### `PATCH` `/v1/supported-languages/games/{gameId}/languages/{languageCode}/universe-display-info-automatic-translation-settings`

**Parameters:**

- `gameId` (path, integer (required)) - The game id.
- `languageCode` (path, string (required)) - The language code.

**Request Body:** Whether to enable automatic translation for universe display info.

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id 72: Automatic translation cannot be enabled for game.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `500` - 77: Content localization set settings return error code invalid 79: Invalid content instance settin

### `GET` `/v1/supported-languages/games/{gameId}/universe-display-info-automatic-translation-settings`

**Parameters:**

- `gameId` (path, integer (required)) - The game id.

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id
- `401` - 0: Authorization has been denied for this request.
- `403` - 18: You do not have permission to manage this game
- `500` - 0: An unknown error occurred. 22: Invalid language code 83: Failed to get UniverseDisplayInformati

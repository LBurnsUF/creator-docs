---
title: V1 / Autolocalization / Games
type: cloud-api
tags: [Localization, Universes]
---

# V1 / Autolocalization / Games

Cloud API resource group with 6 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `PATCH` | `/v1/autolocalization/games/{gameId}/autolocalizationtable` | Use the Autolocalization controller in LocalizationTables API **DEPRECATED** |
| `POST` | `/v1/autolocalization/games/{gameId}/autolocalizationtable` | Use the Autolocalization controller in LocalizationTables API **DEPRECATED** |
| `PATCH` | `/v1/autolocalization/games/{gameId}/autolocalizationtable#LocalizationTablesApi` |  |
| `POST` | `/v1/autolocalization/games/{gameId}/autolocalizationtable#LocalizationTablesApi` |  |
| `PATCH` | `/v1/autolocalization/games/{gameId}/settings` | Sets a game's auto-localization related settings **DEPRECATED** |
| `PATCH` | `/v1/autolocalization/games/{gameId}/settings#LocalizationTablesApi` | Sets a game's auto-localization related settings |

### `PATCH` `/v1/autolocalization/games/{gameId}/autolocalizationtable`

> **Deprecated**

Use the Autolocalization controller in LocalizationTables API

**Parameters:**

- `gameId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

### `POST` `/v1/autolocalization/games/{gameId}/autolocalizationtable`

> **Deprecated**

Use the Autolocalization controller in LocalizationTables API

**Parameters:**

- `gameId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

### `PATCH` `/v1/autolocalization/games/{gameId}/autolocalizationtable#LocalizationTablesApi`

**Parameters:**

- `gameId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

### `POST` `/v1/autolocalization/games/{gameId}/autolocalizationtable#LocalizationTablesApi`

**Parameters:**

- `gameId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

### `PATCH` `/v1/autolocalization/games/{gameId}/settings`

> **Deprecated**

Use the Autolocalization controller in LocalizationTables API

**Parameters:**

- `gameId` (path, integer (required)) - The id of the game.

**Request Body:** The request body.

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `503` - 17: Feature is disabled

### `PATCH` `/v1/autolocalization/games/{gameId}/settings#LocalizationTablesApi`

**Parameters:**

- `gameId` (path, integer (required)) - The id of the game.

**Request Body:** The request body.

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id 61: IsAutomaticEntriesSettingEnabled can only be enabled if IsAutolocalizationE
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `503` - 17: Feature is disabled

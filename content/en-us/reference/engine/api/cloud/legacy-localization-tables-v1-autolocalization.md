---
title: Legacy Localization Tables / V1 / Autolocalization
type: cloud-api
tags: [Localization, Metadata, Universes]
---

# Legacy Localization Tables / V1 / Autolocalization

Cloud API resource group with 3 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/legacy-localization-tables/v1/autolocalization/games/{gameId}/autolocalizationtable` |  |
| `PATCH` | `/legacy-localization-tables/v1/autolocalization/games/{gameId}/settings` | Sets a game's auto-localization related settings |
| `GET` | `/legacy-localization-tables/v1/autolocalization/metadata` | Metadata for AutoLocalization Configuration |

### `POST` `/legacy-localization-tables/v1/autolocalization/games/{gameId}/autolocalizationtable`

**Parameters:**

- `gameId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

### `PATCH` `/legacy-localization-tables/v1/autolocalization/games/{gameId}/settings`

**Parameters:**

- `gameId` (path, integer (required)) - The id of the game.

**Request Body:** The request body.

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id 61: IsAutomaticEntriesSettingEnabled can only be enabled if IsAutolocalizationE
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `503` - 17: Feature is disabled

### `GET` `/legacy-localization-tables/v1/autolocalization/metadata`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

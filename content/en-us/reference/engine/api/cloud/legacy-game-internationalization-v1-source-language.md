---
title: Legacy Game Internationalization / V1 / Source Language
type: cloud-api
tags: [Localization, Universes]
---

# Legacy Game Internationalization / V1 / Source Language

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `PATCH` | `/legacy-game-internationalization/v1/source-language/games/{gameId}` | Sets the source language of a game |

### `PATCH` `/legacy-game-internationalization/v1/source-language/games/{gameId}`

**Parameters:**

- `gameId` (path, integer (required)) - 
- `languageCode` (query, string (required)) - 

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id 22: Invalid language code
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `500` - 85: Failed to disable automatic translation status for languages
- `503` - 17: Feature is disabled

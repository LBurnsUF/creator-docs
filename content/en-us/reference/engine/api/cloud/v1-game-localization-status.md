---
title: V1 / Game Localization Status
type: cloud-api
tags: [Localization, Universes]
---

# V1 / Game Localization Status

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/game-localization-status/{gameId}/translation-counts` | Gets the language translation counts for all languages of a game |

### `GET` `/v1/game-localization-status/{gameId}/translation-counts`

**Parameters:**

- `gameId` (path, integer (required)) - GameID of the game to get translation counts for

**Responses:**

- `200` - OK
- `400` - 4: Table does not exist. 14: Invalid game id
- `401` - 0: Authorization has been denied for this request.
- `500` - 0: An unknown error occurred.

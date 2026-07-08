---
title: V2 / Supported Languages / Games
type: cloud-api
tags: [Universes]
---

# V2 / Supported Languages / Games

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/supported-languages/games/{gameId}` | Get the supported languages for a game. |

### `GET` `/v2/supported-languages/games/{gameId}`

**Parameters:**

- `gameId` (path, integer (required)) - The id of the game.

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id
- `503` - 17: Feature is disabled

---
title: V1 / Automatic Translation / Games
type: cloud-api
tags: [Localization, Universes]
---

# V1 / Automatic Translation / Games

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/automatic-translation/games/{gameId}/feature-status` | Checks if automatic translation can be enabled for a game. The user must still have proper permissi |
| `GET` | `/v1/automatic-translation/games/{gameId}/quota` | Returns the automatic translation quota info for a game. The user must still have proper permission |

### `GET` `/v1/automatic-translation/games/{gameId}/feature-status`

**Parameters:**

- `gameId` (path, integer (required)) - The game id.

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 18: You do not have permission to manage this game
- `503` - 17: Feature is disabled

### `GET` `/v1/automatic-translation/games/{gameId}/quota`

**Parameters:**

- `gameId` (path, integer (required)) - The game id.

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id
- `401` - 0: Authorization has been denied for this request.
- `403` - 18: You do not have permission to manage this game
- `503` - 17: Feature is disabled

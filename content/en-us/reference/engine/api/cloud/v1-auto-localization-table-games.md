---
title: V1 / Auto Localization Table / Games
type: cloud-api
tags: [Localization, Universes]
---

# V1 / Auto Localization Table / Games

Cloud API resource group with 3 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/auto-localization-table/games/{gameId}/assets-generation-request` | Generates localization asset of a game. |
| `POST` | `/v1/auto-localization-table/games/{gameId}/auto-scrape-cleanup-request` | Enqueues an event to flush the auto scraped entries which doesn't have translations. |
| `PATCH` | `/v1/auto-localization-table/games/{gameId}/ingestion` | Ingests entries for auto localization. Needs to be an authorized user. |

### `POST` `/v1/auto-localization-table/games/{gameId}/assets-generation-request`

**Parameters:**

- `gameId` (path, integer (required)) - The game id.

**Responses:**

- `200` - OK
- `400` - 3: Invalid table id. 14: Invalid game id 29: You do not have permission to generate asset for this
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `429` - 24: Too many attempts.Please try again later.

### `POST` `/v1/auto-localization-table/games/{gameId}/auto-scrape-cleanup-request`

**Parameters:**

- `gameId` (path, integer (required)) - The id of the game.

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id 31: You do not have permission to flush auto scraped entries asset for this gam
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `429` - 33: Too many attempts to flush the game.Please try again later.

### `PATCH` `/v1/auto-localization-table/games/{gameId}/ingestion`

**Parameters:**

- `gameId` (path, integer (required)) - The game id.

**Responses:**

- `200` - OK
- `400` - 10: Maximum entries exceeded. Please keep the number of entries per request below the maximum. 13: 
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `503` - 17: Feature is disabled

---
title: Game Passes / V1 / Universes
type: cloud-api
tags: [Game passes]
---

# Game Passes / V1 / Universes

Cloud API resource group with 4 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/game-passes/v1/universes/{universeId}/game-passes` | Create game pass [BETA] |
| `GET` | `/game-passes/v1/universes/{universeId}/game-passes/creator` | List game passes by universe with configuration details [BETA] |
| `PATCH` | `/game-passes/v1/universes/{universeId}/game-passes/{gamePassId}` | Update game pass [BETA] |
| `GET` | `/game-passes/v1/universes/{universeId}/game-passes/{gamePassId}/creator` | Get game pass with configuration details [BETA] |

### `POST` `/game-passes/v1/universes/{universeId}/game-passes`

**Operation:** `GamePasses_CreateGamePass`

**Stability:** BETA

Creates a new game pass with the provided configuration details.

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID.

**Responses:**

- `200` - Success
- `400` - Bad Request
- `401` - Unauthorized
- `403` - Forbidden
- `404` - Not Found

### `GET` `/game-passes/v1/universes/{universeId}/game-passes/creator`

**Operation:** `GamePasses_ListGamePassConfigsByUniverse`

**Stability:** BETA

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID.
- `pageSize` (query, integer) - The number of results to return. Defaults to 50 if not provided.
- `pageToken` (query, string) - The cursor token for pagination.

**Responses:**

- `200` - Success
- `400` - Bad Request
- `401` - Unauthorized
- `403` - Forbidden
- `404` - Not Found

### `PATCH` `/game-passes/v1/universes/{universeId}/game-passes/{gamePassId}`

**Operation:** `GamePasses_UpdateGamePass`

**Stability:** BETA

Updates a game pass with the provided configuration details.
Note that only fields provided in the request will be updated.

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID.
- `gamePassId` (path, integer (required)) - The game pass ID.

**Responses:**

- `204` - No Content
- `400` - Bad Request
- `401` - Unauthorized
- `403` - Forbidden
- `404` - Not Found
- `409` - Conflict

### `GET` `/game-passes/v1/universes/{universeId}/game-passes/{gamePassId}/creator`

**Operation:** `GamePasses_GetGamePassConfig`

**Stability:** BETA

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID.
- `gamePassId` (path, integer (required)) - The game pass ID.

**Responses:**

- `200` - Success
- `401` - Unauthorized
- `403` - Forbidden
- `404` - Not Found

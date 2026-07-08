---
title: V1 / Game Localization Roles / Games
type: cloud-api
tags: [Localization, Universes, Users]
---

# V1 / Game Localization Roles / Games

Cloud API resource group with 3 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `PATCH` | `/v1/game-localization-roles/games/{gameId}` | Assigns or revokes a role |
| `GET` | `/v1/game-localization-roles/games/{gameId}/current-user/roles` | Retrieves the list of roles granted to current logged-in user |
| `GET` | `/v1/game-localization-roles/games/{gameId}/roles/{role}/assignees` | Gets list of users assigned a specific role in a game. |

### `PATCH` `/v1/game-localization-roles/games/{gameId}`

**Parameters:**

- `gameId` (path, integer (required)) - The id of the game

**Request Body:** The request body

**Responses:**

- `200` - OK
- `400` - 3: Invalid game id 4: Invalid assignee id 6: Request body can't be null 7: The role you are assig
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 1: You must be authorized to use this endpoint
- `429` - 5: Too many attempts. Please try again later.
- `503` - 2: Feature is disabled

### `GET` `/v1/game-localization-roles/games/{gameId}/current-user/roles`

**Parameters:**

- `gameId` (path, integer (required)) - The id of the game

**Responses:**

- `200` - OK
- `400` - 3: Invalid game id
- `401` - 0: Authorization has been denied for this request.
- `503` - 2: Feature is disabled

### `GET` `/v1/game-localization-roles/games/{gameId}/roles/{role}/assignees`

**Parameters:**

- `gameId` (path, integer (required)) - The id of the game
- `role` (path, string (required)) - The Roblox.GameLocalization.Client.GameLocalizationRoles.GameLocalizationRoleType

**Responses:**

- `200` - OK
- `400` - 3: Invalid game id
- `401` - 0: Authorization has been denied for this request.
- `403` - 1: You must be authorized to use this endpoint
- `503` - 2: Feature is disabled

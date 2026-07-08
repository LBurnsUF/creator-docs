---
title: V1 / Avatar / Set Player Avatar Type
type: cloud-api
tags: [Avatars]
---

# V1 / Avatar / Set Player Avatar Type

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/avatar/set-player-avatar-type` | Sets the authenticated user's player avatar type (e.g. R6 or R15). |

### `POST` `/v1/avatar/set-player-avatar-type`

This is the avatar type chosen on the Avatar page. Some games can override this and force your character to be R6 or R15.

**Parameters:**

- `Roblox-Place-Id` (header, integer) - 

**Request Body:** R6 or R15.

**Responses:**

- `200` - OK
- `400` - 1: Invalid playerAvatarType. Valid values are: 
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: You are not allowed to change player avatar type.

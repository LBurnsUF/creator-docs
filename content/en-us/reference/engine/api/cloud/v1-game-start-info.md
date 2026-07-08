---
title: V1 / Game Start Info
type: cloud-api
tags: [Avatars, Universes]
---

# V1 / Game Start Info

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/game-start-info` | The server will call this on game server start to request general information about the universe Th |

### `GET` `/v1/game-start-info`

**Parameters:**

- `universeId` (query, integer (required)) - 
- `Roblox-Place-Id` (header, integer) - 

**Responses:**

- `200` - OK

---
title: Matchmaking Api / V1 / Game Instances
type: cloud-api
tags: [Matchmaking]
---

# Matchmaking Api / V1 / Game Instances

Cloud API resource group with 5 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/matchmaking-api/v1/game-instances/forecast-update` | Forecast the outcome of launching an update [BETA] |
| `GET` | `/matchmaking-api/v1/game-instances/get-update-status` | Get the rollout status of an update [BETA] |
| `POST` | `/matchmaking-api/v1/game-instances/launch-update` | Launch a game update [BETA] |
| `POST` | `/matchmaking-api/v1/game-instances/shutdown` | Shutdown game instances. [BETA] |
| `POST` | `/matchmaking-api/v1/game-instances/shutdown-all` | Shutdown all game instances. [BETA] |

### `POST` `/matchmaking-api/v1/game-instances/forecast-update`

**Stability:** BETA

**Responses:**

- `200` - Success

### `GET` `/matchmaking-api/v1/game-instances/get-update-status`

**Stability:** BETA

**Parameters:**

- `universeId` (query, integer) - 

**Responses:**

- `200` - Success

### `POST` `/matchmaking-api/v1/game-instances/launch-update`

**Stability:** BETA

**Responses:**

- `200` - Success

### `POST` `/matchmaking-api/v1/game-instances/shutdown`

**Stability:** BETA

**Responses:**

- `200` - Success

### `POST` `/matchmaking-api/v1/game-instances/shutdown-all`

**Stability:** BETA

**Responses:**

- `200` - Success

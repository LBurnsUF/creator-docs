---
title: Matchmaking Api / V1 / Client Status
type: cloud-api
tags: [Matchmaking]
---

# Matchmaking Api / V1 / Client Status

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/matchmaking-api/v1/client-status` | Get the client-status [BETA] |
| `POST` | `/matchmaking-api/v1/client-status` | Set the client-status [BETA] |

### `GET` `/matchmaking-api/v1/client-status`

**Stability:** BETA

**Request Body:** ClientStatusGetRequest

**Responses:**

- `200` - Success

### `POST` `/matchmaking-api/v1/client-status`

**Stability:** BETA

**Request Body:** ClientStatusSetRequest

**Responses:**

- `200` - Success

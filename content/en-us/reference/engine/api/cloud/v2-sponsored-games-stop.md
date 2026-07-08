---
title: V2 / Sponsored Games / Stop
type: cloud-api
tags: [Sponsored campaigns]
---

# V2 / Sponsored Games / Stop

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v2/sponsored-games/stop` | To stop a sponsored-game ad (ad set) from running, initiated by a user. |

### `POST` `/v2/sponsored-games/stop`

**Request Body:** Roblox.AdConfiguration.Api.Models.StopSponsoredGameV2Request

**Responses:**

- `200` - OK
- `400` - 14: Invalid ad set id.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 10: Insufficient permissions.
- `503` - 1: This feature is disabled.

---
title: V2 / Sponsored Campaigns / Stop
type: cloud-api
tags: [Sponsored campaigns]
---

# V2 / Sponsored Campaigns / Stop

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v2/sponsored-campaigns/stop` | Stops a sponsored campaign / ad (ad set) from running. Initiated by a user. |

### `POST` `/v2/sponsored-campaigns/stop`

**Request Body:** Roblox.AdConfiguration.Api.Models.StopSponsoredCampaignRequest

**Responses:**

- `200` - OK
- `400` - 10: Insufficient permissions. 14: Invalid ad set id. 31: Internal server error
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `503` - 1: This feature is disabled.

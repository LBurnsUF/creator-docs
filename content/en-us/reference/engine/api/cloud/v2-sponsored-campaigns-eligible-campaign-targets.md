---
title: V2 / Sponsored Campaigns / Eligible Campaign Targets
type: cloud-api
tags: [Sponsored campaigns]
---

# V2 / Sponsored Campaigns / Eligible Campaign Targets

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v2/sponsored-campaigns/eligible-campaign-targets` | Returns a collection of Roblox.AdConfiguration.Api.Models.CampaignTargetModel that the user is autho |

### `POST` `/v2/sponsored-campaigns/eligible-campaign-targets`

**Request Body:** Roblox.AdConfiguration.Api.Models.GetEligibleCampaignTargetsRequest

**Responses:**

- `200` - OK
- `400` - 19: Invalid group id.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 10: Insufficient permissions.

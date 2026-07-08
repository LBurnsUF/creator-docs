---
title: V2 / Sponsored Campaigns / Create
type: cloud-api
tags: [Sponsored campaigns]
---

# V2 / Sponsored Campaigns / Create

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v2/sponsored-campaigns/create` | Creates a complete ad. Including ad campaign, ad set, escrow, and the ad. Currently intended for cr |

### `POST` `/v2/sponsored-campaigns/create`

**Request Body:** Roblox.AdConfiguration.Api.Models.CreateSponsoredCampaignRequest

**Responses:**

- `200` - OK
- `400` - 2: Daily budget is lower than minimum allowed. 3: Total budget must be greater than 0. 4: Ad name 
- `401` - 0: Authorization has been denied for this request. 10: Insufficient permissions.
- `403` - 0: Token Validation Failed
- `500` - 0: An unknown error occurred. 31: Internal server error
- `503` - 1: This feature is disabled.

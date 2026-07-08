---
title: V2 / Sponsored Games / Create
type: cloud-api
tags: [Sponsored campaigns]
---

# V2 / Sponsored Games / Create

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v2/sponsored-games/create` | Creates a new sponsored game ad with specified input parameters. |

### `POST` `/v2/sponsored-games/create`

**Request Body:** Roblox.AdConfiguration.Api.CreateSponsoredGameV2Request

**Responses:**

- `200` - OK
- `400` - 2: Daily budget is lower than minimum allowed. 3: Total budget must be greater than 0. 4: Ad name 
- `401` - 0: Authorization has been denied for this request. 10: Insufficient permissions.
- `403` - 0: Token Validation Failed
- `500` - 0: An unknown error occurred. 31: Internal server error
- `503` - 1: This feature is disabled.

---
title: V2 / Sponsored Games
type: cloud-api
tags: [Sponsored campaigns]
---

# V2 / Sponsored Games

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/sponsored-games` | Gets a page of Roblox.AdConfiguration.Api.SponsoredGameV2Model with specified input parameters. |

### `GET` `/v2/sponsored-games`

**Parameters:**

- `universeId` (query, integer (required)) - The universe id of the ad campaign.
- `includeReportingStats` (query, boolean) - Indicates whether to include reporting stats in the response.
- `isArchived` (query, boolean) - Indicates whether to retrieve archived ads.
- `pageCursor` (query, string) - The cursor of the page to retrieve.

**Responses:**

- `200` - OK
- `400` - 9: Cannot load the universe for the specified universe id. 9: Cannot load the universe for the spec
- `401` - 0: Authorization has been denied for this request.
- `503` - 1: This feature is disabled.

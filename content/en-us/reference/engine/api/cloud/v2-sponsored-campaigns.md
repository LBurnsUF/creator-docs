---
title: V2 / Sponsored Campaigns
type: cloud-api
tags: [Sponsored campaigns]
---

# V2 / Sponsored Campaigns

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/sponsored-campaigns` | Gets a page of Roblox.AdConfiguration.Api.SponsoredCampaignModel with specified input parameters. |

### `GET` `/v2/sponsored-campaigns`

**Parameters:**

- `campaignTargetType` (query, integer (required)) - The campaign target type enum value
- `campaignTargetId` (query, integer (required)) - The id of the campaign target
- `includeReportingStats` (query, boolean) - Indicates whether to include reporting stats in the response
- `isArchived` (query, boolean) - Indicates whether to retrieve archived ads
- `pageCursor` (query, string) - The cursor of the page to retrieve. If empty, fetches the first page

**Responses:**

- `200` - OK
- `400` - 22: Invalid campaign target ID. 23: Invalid campaign target type.
- `401` - 0: Authorization has been denied for this request.
- `503` - 1: This feature is disabled.

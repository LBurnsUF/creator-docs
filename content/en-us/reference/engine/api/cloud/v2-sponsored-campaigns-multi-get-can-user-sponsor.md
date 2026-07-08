---
title: V2 / Sponsored Campaigns / Multi Get Can User Sponsor
type: cloud-api
tags: [Sponsored campaigns]
---

# V2 / Sponsored Campaigns / Multi Get Can User Sponsor

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/sponsored-campaigns/multi-get-can-user-sponsor` | Checks whether the targets are eligible for sponsorship, and if the user is authorized to sponsor t |

### `GET` `/v2/sponsored-campaigns/multi-get-can-user-sponsor`

**Parameters:**

- `campaignTargetType` (query, integer (required)) - Ads.Management.Service.CampaignTargetType.
- `campaignTargetIds` (query, array (required)) - The IDs of the campaign targets.

**Responses:**

- `200` - OK
- `400` - Bad Request
- `401` - 0: Authorization has been denied for this request.
- `403` - Forbidden
- `500` - Server Error

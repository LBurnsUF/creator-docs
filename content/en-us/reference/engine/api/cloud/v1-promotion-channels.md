---
title: V1 / Promotion Channels
type: cloud-api
tags: [Accounts, User profiles]
---

# V1 / Promotion Channels

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/promotion-channels` | Get the user's promotion channels |
| `POST` | `/v1/promotion-channels` | Update the user's promotion channels |

### `GET` `/v1/promotion-channels`

**Parameters:**

- `alwaysReturnUrls` (query, boolean) - Whether all promotion channel links should be returned as full URLs.
- `filterLink` (query, boolean) - Whether all promotion channel links should be filtered.
- `onlyShortenTwitter` (query, boolean) - Whether all promotion channels links except for Twitter should be returned as full URLs. If false, all promotion channels will be shortened.

**Responses:**

- `200` - OK
- `400` - 1: User not found.
- `401` - 0: Authorization has been denied for this request.

### `POST` `/v1/promotion-channels`

**Request Body:** The Roblox.AccountInformation.Api.Models.PromotionChannelsRequest

**Responses:**

- `200` - OK
- `400` - 2: The request was empty. 11: The Facebook profile url is invalid. 12: The Twitter handle is inval
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 4: Only users who are over twelve years of age may edit social network c

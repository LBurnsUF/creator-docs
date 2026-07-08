---
title: V2 / Avatar / Set Wearing Assets
type: cloud-api
tags: [Avatars]
---

# V2 / Avatar / Set Wearing Assets

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v2/avatar/set-wearing-assets` | Sets the avatar's current assets to the list. |

### `POST` `/v2/avatar/set-wearing-assets`

Only allows items that you own, are not expired, and are wearable asset types.
Any assets being worn before this method is called are automatically removed.

**Parameters:**

- `Roblox-Place-Id` (header, integer) - 

**Request Body:** Model of assets to be worn.

**Responses:**

- `200` - OK
- `400` - 3: Invalid assetId 5: Meta does not apply to specified asset type 7: Required meta is not provided
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `500` - 2: Failed to wear asset.

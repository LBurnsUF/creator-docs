---
title: V3 / Outfits
type: cloud-api
tags: [Avatars]
---

# V3 / Outfits

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `PATCH` | `/v3/outfits/{userOutfitId}` | Updates the contents of an outfit. |
| `GET` | `/v3/outfits/{userOutfitId}/details` | Gets details about the contents of an outfit. |

### `PATCH` `/v3/outfits/{userOutfitId}`

Fails if the user does not own any of the assetIds or if they are not wearable asset types.
Accepts partial updates.

**Parameters:**

- `userOutfitId` (path, integer (required)) - The user outfit id.
- `Roblox-Place-Id` (header, integer) - 

**Request Body:** The updated outfit.

**Responses:**

- `200` - OK
- `400` - 3: Body colors must be valid BrickColor IDs 4: Invalid outfit name 5: Asset is not wearable by you
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: You don't have permission to update this outfit.
- `404` - 1: The specified userOutfit does not exist!
- `500` - 6: An error occurred while trying to update the outfit

### `GET` `/v3/outfits/{userOutfitId}/details`

**Parameters:**

- `userOutfitId` (path, integer (required)) - The user outfit id.
- `Roblox-Place-Id` (header, integer) - 
- `checkAssetAvailability` (query, boolean) - Whether to return assets with availability status.

**Responses:**

- `200` - OK
- `400` - 2: The outfit for the specified userOutfit is invalid.
- `403` - 3: The requester does not have access to the details for the given user outfit.
- `404` - 1: The specified userOutfitId is invalid.

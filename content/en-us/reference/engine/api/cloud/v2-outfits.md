---
title: V2 / Outfits
type: cloud-api
tags: [Avatars]
---

# V2 / Outfits

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `PATCH` | `/v2/outfits/{userOutfitId}` | Updates the contents of an outfit. **DEPRECATED** |

### `PATCH` `/v2/outfits/{userOutfitId}`

> **Deprecated**

Fails if the user does not own any of the assetIds or if they are not wearable asset types.
Accepts partial updates.

Please use PATCH v3/outfits/{userOutfitId}

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

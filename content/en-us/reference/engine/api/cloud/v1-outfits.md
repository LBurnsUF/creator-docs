---
title: V1 / Outfits
type: cloud-api
tags: [Avatars]
---

# V1 / Outfits

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/outfits/{userOutfitId}/delete` | Deletes the outfit. |
| `GET` | `/v1/outfits/{userOutfitId}/details` | Gets details about the contents of an outfit. |

### `POST` `/v1/outfits/{userOutfitId}/delete`

You are only allowed to delete outfits you created.

**Parameters:**

- `userOutfitId` (path, integer (required)) - The user outfit id.
- `Roblox-Place-Id` (header, integer) - 

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: You don't have permission to delete this outfit.
- `404` - 1: The specified userOutfitId is invalid!
- `500` - 3: An error occurred while deleting the outfit.

### `GET` `/v1/outfits/{userOutfitId}/details`

**Parameters:**

- `userOutfitId` (path, integer (required)) - The user outfit id.
- `Roblox-Place-Id` (header, integer) - 

**Responses:**

- `200` - OK
- `400` - 2: The outfit for the specified userOutfit is invalid.
- `403` - 3: The requester does not have access to the details for the given user outfit.
- `404` - 1: The specified userOutfitId is invalid.

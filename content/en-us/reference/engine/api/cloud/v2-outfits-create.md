---
title: V2 / Outfits / Create
type: cloud-api
tags: [Avatars]
---

# V2 / Outfits / Create

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v2/outfits/create` | Creates a new outfit. **DEPRECATED** |

### `POST` `/v2/outfits/create`

> **Deprecated**

Fails if any of the assetIds are not owned by the user, or not wearable types.
The name property of the request is optional as one will be auto-generated when the request has a null name.

please use v3/outfits/create

**Parameters:**

- `Roblox-Place-Id` (header, integer) - 

**Request Body:** The new outfit.

**Responses:**

- `200` - OK
- `400` - 3: Body colors must be valid BrickColor IDs 4: Invalid outfit name 5: Asset is not wearable by you
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 1: You already have the maximum number of outfits
- `500` - 6: An error occurred while creating the outfit

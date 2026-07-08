---
title: V2 / Universes
type: cloud-api
tags: [Universes]
---

# V2 / Universes

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `PATCH` | `/v2/universes/{universeId}/configuration` | Update universe settings for an owned universe. V2 Contains data for avatar scale and asset overrid |

### `PATCH` `/v2/universes/{universeId}/configuration`

**Parameters:**

- `universeId` (path, integer (required)) - The universeId.

**Request Body:** The Roblox.Api.Develop.Models.UniverseSettingsRequest model.

**Responses:**

- `200` - OK
- `400` - 1: The universe does not exist. 3: Invalid UniverseAvatarType. 4: Invalid UniverseScaleType. 5: I
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: You are not authorized to configure this universe. 14: You are not a
- `409` - 9: Failed to shutdown all intances of game after changing AvatarType. The change has been reverted.
- `500` - 43: Failed to update the audience configuration. The change was not applied. Please try again.

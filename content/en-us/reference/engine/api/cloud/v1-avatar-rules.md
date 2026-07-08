---
title: V1 / Avatar Rules
type: cloud-api
tags: [Avatars]
---

# V1 / Avatar Rules

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/avatar-rules` | Returns the business rules related to avatars. |

### `GET` `/v1/avatar-rules`

BodyColorsPalette is a list of valid brickColors you can choose for your avatar.
WearableAssetTypes contains a list of asset types with names, ids, and the maximum number that you can wear at a time.
Does not include packages because they cannot be worn on your avatar directly.
PlayerAvatarTypes are the types of avatars you can choose between.

**Parameters:**

- `Roblox-Place-Id` (header, integer) - 

**Responses:**

- `200` - OK

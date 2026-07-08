---
title: V2 / Avatar / Users
type: cloud-api
tags: [Avatars, Users]
---

# V2 / Avatar / Users

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/avatar/users/{userId}/avatar` | Returns details about a specified user's avatar. |
| `GET` | `/v2/avatar/users/{userId}/outfits` | Gets a list of outfits for the specified user. |

### `GET` `/v2/avatar/users/{userId}/avatar`

Includes assets, bodycolors, and playerAvatarType.

**Parameters:**

- `userId` (path, integer (required)) - 
- `Roblox-Place-Id` (header, integer) - 
- `checkAssetAvailability` (query, boolean) - Whether to return assets with availability status.

**Responses:**

- `200` - OK
- `400` - 1: The specified user does not exist. 2: An account for the given userId does not exist!

### `GET` `/v2/avatar/users/{userId}/outfits`

**Parameters:**

- `userId` (path, integer (required)) - The user id.
- `paginationToken` (query, string) - The token received from the response to get the next page. For the first request, this value should be empty. Note : If no value is sent the 1st page 
- `outfitType` (query, string) - The outfit type being searched for, null will return all outfitTypes.
- `page` (query, integer) - The page number of the current page of requests, default is 1.
- `itemsPerPage` (query, integer) - The max number of outfits that can be returned.
- `isEditable` (query, boolean) - Whether the outfits are editable. A null value will lead to no filtering.
- `Roblox-Place-Id` (header, integer) - The placeId of the caller, not required to be passed in.

**Responses:**

- `200` - OK
- `400` - 1: The specified user does not exist. 2: An account for the given userId does not exist!

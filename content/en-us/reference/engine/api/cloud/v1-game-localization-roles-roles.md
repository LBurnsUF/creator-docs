---
title: V1 / Game Localization Roles / Roles
type: cloud-api
tags: [Localization, Universes]
---

# V1 / Game Localization Roles / Roles

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/game-localization-roles/roles/{role}/current-user` | Gets the list of games and associated role assignment info for the requested user and role. |

### `GET` `/v1/game-localization-roles/roles/{role}/current-user`

**Parameters:**

- `role` (path, string (required)) - The Roblox.GameLocalization.Client.GameLocalizationRoles.GameLocalizationRoleType
- `exclusiveStartKey` (query, string) - Part of pagination. Last primary key of returned items in previous operation.
- `pageSize` (query, integer) - Part of pagination. Maximum number of items that might be returned in the page.
- `groupId` (query, integer) - Optional seleted groupId of resources requested for the user and role.

**Responses:**

- `200` - OK
- `400` - 10: Invalid page size 11: Maximum page size exceeded 12: Invalid exclusive start key
- `401` - 0: Authorization has been denied for this request.
- `500` - 0: An unknown error occurred
- `503` - 2: Feature is disabled

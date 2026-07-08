---
title: V1 / Universes / Multiget
type: cloud-api
tags: [Team Create, Universes]
---

# V1 / Universes / Multiget

Cloud API resource group with 3 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/universes/multiget` | Gets a list of universes. |
| `GET` | `/v1/universes/multiget/permissions` | Returns an array of granted and declined permissions related to the universes with the ids in ids fo |
| `GET` | `/v1/universes/multiget/teamcreate` | Gets TeamCreate settings for multiple universes specified by Ids |

### `GET` `/v1/universes/multiget`

If a universe can not be found for a given ID (such as -1) it will be skipped.

**Parameters:**

- `ids` (query, array (required)) - The universe IDs to get. Limit 100.

**Responses:**

- `200` - OK
- `400` - 8: No universe IDs sent to get. 9: Too many universe IDs sent to get, the limit is: 

### `GET` `/v1/universes/multiget/permissions`

If a universe can not be found for a given ID (such as -1) it will be skipped.

**Parameters:**

- `ids` (query, array (required)) - The universe ids.

**Responses:**

- `200` - OK
- `400` - 8: No universe IDs sent to get. 9: Too many universe IDs sent to get, the limit is: 
- `401` - 0: Authorization has been denied for this request.

### `GET` `/v1/universes/multiget/teamcreate`

**Parameters:**

- `ids` (query, array (required)) - The universe Ids.

**Responses:**

- `200` - OK
- `400` - Roblox.Api.Develop.ResponseEnums.TeamCreateErrors.TooManyUniverseIdsSent
- `401` - 0: Authorization has been denied for this request.

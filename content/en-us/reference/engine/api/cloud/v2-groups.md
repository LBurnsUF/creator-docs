---
title: V2 / Groups
type: cloud-api
tags: [Groups, Universes]
---

# V2 / Groups

Cloud API resource group with 4 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/groups` | Multi-get groups information by Ids. |
| `GET` | `/v2/groups/{groupId}/games` | Gets experiences created by the specified group id. |
| `GET` | `/v2/groups/{groupId}/gamesV2` | Gets experiences created by the specified group id. |
| `GET` | `/v2/groups/{groupId}/transactions` |  |

### `GET` `/v2/groups`

If a group comes back as null, it will not be returned in the response.

**Parameters:**

- `groupIds` (query, array (required)) - The group Ids.

**Responses:**

- `200` - OK
- `400` - 2: Too many ids in request. 3: Ids could not be parsed from request.

### `GET` `/v2/groups/{groupId}/games`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id
- `accessFilter` (query, integer) - The access type of the experiences.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `501` - 47: Code path is not implemented.

### `GET` `/v2/groups/{groupId}/gamesV2`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id
- `accessFilter` (query, integer) - The access type of the experiences.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `501` - 47: Code path is not implemented.

### `GET` `/v2/groups/{groupId}/transactions`

**Operation:** `TransactionHistory_GetGroupTransactions`

**Parameters:**

- `groupId` (path, integer (required)) - 
- `exclusiveStartRequest` (query) - 
- `transactionType` (query) - 

**Responses:**

- `200` - Success

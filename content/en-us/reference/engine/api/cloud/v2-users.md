---
title: V2 / Users
type: cloud-api
tags: [Assets, Groups, Interactions, Inventories, Trades, Universes, Users]
---

# V2 / Users

Cloud API resource group with 11 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/users/{userId}/can-trade-with` | Checks if the user can trade with a specific user. |
| `GET` | `/v2/users/{userId}/favorite/games` | Gets users favorite games. |
| `GET` | `/v2/users/{userId}/games` | Gets games created by the specified user. |
| `GET` | `/v2/users/{userId}/groups/roles` | Gets a list of all group roles for groups the specified user is in. |
| `GET` | `/v2/users/{userId}/inventory` | Get user's inventory by multiple Roblox.Platform.Assets.AssetType. |
| `GET` | `/v2/users/{userId}/inventory/{assetTypeId}` | Gets user's inventory based on specific asset type |
| `GET` | `/v2/users/{userId}/tradableItems` | Gets tradable items for a user. |
| `GET` | `/v2/users/{userId}/transaction-totals` |  |
| `GET` | `/v2/users/{userId}/transaction-types` |  |
| `GET` | `/v2/users/{userId}/transactions` |  |
| `GET` | `/v2/users/{userId}/universes` | Gets all universes followed by a user. |

### `GET` `/v2/users/{userId}/can-trade-with`

**Parameters:**

- `userId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request. 4: You are not authorized to modify this trade.

### `GET` `/v2/users/{userId}/favorite/games`

**Parameters:**

- `userId` (path, integer (required)) - The user Id.
- `accessFilter` (query, integer) - Filtering option via access level.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK

### `GET` `/v2/users/{userId}/games`

**Parameters:**

- `userId` (path, integer (required)) - The user Id.
- `accessFilter` (query, integer) - Filtering option via access level.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK

### `GET` `/v2/users/{userId}/groups/roles`

**Parameters:**

- `userId` (path, integer (required)) - The user id.
- `includeLocked` (query, boolean (required)) - 
- `includeNotificationPreferences` (query, boolean (required)) - 
- `discoveryType` (query, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 3: The user is invalid or does not exist.

### `GET` `/v2/users/{userId}/inventory`

GamePass and Badges not allowed.

**Parameters:**

- `userId` (path, integer (required)) - The inventory owner's userId.
- `assetTypes` (query, array (required)) - The asset types to query.
- `filterDisapprovedAssets` (query, boolean) - Filters moderated assets when enabled.
- `showApprovedOnly` (query, boolean) - Filters moderated assets and assets pending review when enabled.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `400` - 1: Invalid user Id. 2: Invalid asset type Id.
- `403` - 3: Insufficient permission. 4: You are not authorized to view this user's inventory.

### `GET` `/v2/users/{userId}/inventory/{assetTypeId}`

**Parameters:**

- `userId` (path, integer (required)) - The user Id of the inventory owner
- `assetTypeId` (path, integer (required)) - The asset type Id of the items to get
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `400` - 1: Invalid user Id. 2: Invalid asset type Id.
- `403` - 3: Insufficient permission. 4: You are not authorized to view this user's inventory.

### `GET` `/v2/users/{userId}/tradableItems`

**Parameters:**

- `userId` (path, integer (required)) - The id of the user.
- `search` (query, string) - Optional search query to filter items by.
- `itemTargetTypes` (query, array) - Optional list of item target types to filter by.
- `sortBy` (query, string) - The key to sort tradable items by.
- `sortOrder` (query, integer) - The sort order for the tradable items.
- `limit` (query, integer) - The maximum number of items to return.
- `cursor` (query, string) - The pagination cursor.

**Responses:**

- `200` - OK
- `400` - 25: The cursor provided is invalid.
- `401` - 0: Authorization has been denied for this request. 4: You are not authorized to modify this trade.
- `403` - 4: You are not authorized to modify this trade.
- `404` - 0: An unknown error occured.

### `GET` `/v2/users/{userId}/transaction-totals`

**Operation:** `TransactionRecords_GetUserRevenueSummary`

**Parameters:**

- `userId` (path, integer (required)) - 
- `usedTypes` (query, integer) - 
- `timeFrame` (query) - 
- `transactionType` (query) - 
- `exclusiveStartCursor` (query) - 

**Responses:**

- `200` - Success

### `GET` `/v2/users/{userId}/transaction-types`

**Operation:** `TransactionRecords_GetUsedTransactionTypes`

**Parameters:**

- `userId` (path, integer (required)) - 

**Responses:**

- `200` - Success

### `GET` `/v2/users/{userId}/transactions`

**Operation:** `TransactionRecordsApi.TransactionRecords_GetUserTransactions`

**Parameters:**

- `userId` (path, integer (required)) - 
- `exclusiveStartCursor` (query) - 
- `transactionType` (query) - 
- `itemPricingType` (query) - 

**Responses:**

- `200` - Success

### `GET` `/v2/users/{userId}/universes`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - User is not authorized for this action.

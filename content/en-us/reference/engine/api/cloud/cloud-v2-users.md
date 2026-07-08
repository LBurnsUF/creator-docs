---
title: Cloud / V2 / Users
type: cloud-api
tags: [Assets, Avatars, Inventories, Notifications, Thumbnails, Users]
---

# Cloud / V2 / Users

Cloud API resource group with 6 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/cloud/v2/users/{user_id}` | Get User [BETA] |
| `GET` | `/cloud/v2/users/{user_id}/asset-quotas` | List Asset Quotas [BETA] |
| `GET` | `/cloud/v2/users/{user_id}/inventory-items` | List Inventory Items [BETA] |
| `POST` | `/cloud/v2/users/{user_id}/notifications` | Create User Notification [STABLE] |
| `GET` | `/cloud/v2/users/{user_id}/operations/{operation_id}` | Get User Thumbnail Generation Operation [BETA] |
| `GET` | `/cloud/v2/users/{user_id}:generateThumbnail` | Generate User Thumbnail [BETA] |

### `GET` `/cloud/v2/users/{user_id}`

**Operation:** `Cloud_GetUser`

**Stability:** BETA

Gets a user's basic and advanced information.

To access a user's public information, no additional scopes are required.

To access a user's verification status, you need the following scopes:
* user.advanced:read

To access a user's social account information, you need the following
scopes:
* user.social:read

**Parameters:**

- `user_id` (path, string (required)) - The user ID.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/users/{user_id}/asset-quotas`

**Operation:** `Cloud_ListAssetQuotas`

**Stability:** BETA

Returns a list of asset quotas.

**Parameters:**

- `user_id` (path, string (required)) - The user ID.
- `maxPageSize` (query, integer) - The maximum number of asset quotas to return. The service might return fewer than this value. If unspecified, at most 10 asset quotas are returned. Th
- `pageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page.  When paginating, all other parameters provided to the subsequent call mus
- `filter` (query, string) - This field may be set in order to filter the resources returned.  Supports the following subset of CEL: * Only the `quotaType` and `assetType` fields 

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/users/{user_id}/inventory-items`

**Operation:** `Cloud_ListInventoryItems`

**Stability:** BETA

List the inventory items in a user's inventory.

The inventory items returned depend on the target user’s choice under
**Settings > Privacy > Who can see my inventory?**:
* If the user granted inventory visibility to "Everyone," then any API key
or OAuth2 token can be used to view the target’s inventory, no matter what
scopes it has or who created it.
* If the user has not granted inventory visibility to "Everyone":
  * Their inventory can still be viewed with an API key created by the
  target user with **Inventory: Read** permission.
  * Their inventory can still be viewed with an OAuth2 token if the target
  user authorizes an app requesting permissions for the
  `user.inventory-item:read` scope.

**Parameters:**

- `user_id` (path, string (required)) - The user ID.
- `maxPageSize` (query, integer) - The maximum number of inventory items to return. The service might return fewer than this value. If unspecified, at most 10 inventory items are return
- `pageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page.  When paginating, all other parameters provided to the subsequent call mus
- `filter` (query, string) - This field may be set in order to filter the resources returned.  See the [filtering](/cloud/reference/patterns#list-inventory-items) documentation fo

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/users/{user_id}/notifications`

**Operation:** `Cloud_CreateUserNotification`

**Stability:** STABLE

Sends a notification to a user.

**Parameters:**

- `user_id` (path, string (required)) - The user ID.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/users/{user_id}/operations/{operation_id}`

**Operation:** `Cloud_GetUserThumbnailGenerationOperation`

**Stability:** BETA

Retrieves the status of the operation to [generate a user thumbnail](https://create.roblox.com/docs/cloud/reference/features/users#Cloud_GenerateUserThumbnail).

**Parameters:**

- `user_id` (path, string (required)) - The user ID.
- `operation_id` (path, string (required)) - The operation ID.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/users/{user_id}:generateThumbnail`

**Operation:** `Cloud_GenerateUserThumbnail`

**Stability:** BETA

Generates and returns the URL for the user's avatar thumbnail.

**Parameters:**

- `user_id` (path, string (required)) - The user ID.
- `size` (query, integer) - Size of the generated thumbnail. The generated thumbnail will have `size * size` dimension.  Currently supported values: 48, 50, 60, 75, 100, 110, 150
- `format` (query, string) - Specify the format of the generated thumbnail. Default is `PNG`.  Possible values:    | Value | Description |   | --- | --- |   | FORMAT_UNSPECIFIED |
- `shape` (query, string) - Specify the shape of the thumbnail. Default is `ROUND` (circular).  Possible values:    | Value | Description |   | --- | --- |   | SHAPE_UNSPECIFIED 

**Responses:**

- `200` - OK

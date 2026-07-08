---
title: V1 / Users
type: cloud-api
tags: [Accounts, Assets, Avatars, Badges, Connections, Groups, Interactions, Inventories, Places, Trades, Universes, User profiles, Users]
---

# V1 / Users

Cloud API resource group with 74 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/users` | Get users by ids. |
| `POST` | `/v1/users/{targetUserId}/follow` | Creates the following between a user and user with targetUserId |
| `GET` | `/v1/users/{targetUserId}/followers` | Get all users that follow user with targetUserId in page response format |
| `GET` | `/v1/users/{targetUserId}/followers/count` | Get the number of following a user has |
| `GET` | `/v1/users/{targetUserId}/followings` | Get all users that user with targetUserId is following in page response format |
| `GET` | `/v1/users/{targetUserId}/followings/count` | Get the number of following a user has |
| `POST` | `/v1/users/{targetUserId}/unfollow` | Deletes the following between a user and user with targetUserId |
| `GET` | `/v1/users/{userId}` | Gets detailed user information by id. |
| `GET` | `/v1/users/{userId}/assets/collectibles` | Gets all collectible assets owned by the specified user. |
| `GET` | `/v1/users/{userId}/avatar` | Returns details about a specified user's avatar. |
| `GET` | `/v1/users/{userId}/badges` | Gets a list of badges a user has been awarded. |
| `GET` | `/v1/users/{userId}/badges/awarded-dates` | Gets timestamps for when badges were awarded to a user. |
| `GET` | `/v1/users/{userId}/badges/{badgeId}/awarded-date` | Gets timestamp for when a single badge was awarded to a user. |
| `GET` | `/v1/users/{userId}/bundles` | Lists the bundles owned by a given user. |
| `GET` | `/v1/users/{userId}/bundles/{bundleType}` |  |
| `GET` | `/v1/users/{userId}/can-trade-with` | Returns whether you can trade with another user. |
| `GET` | `/v1/users/{userId}/can-view-inventory` | Gets whether the specified user's inventory can be viewed. |
| `GET` | `/v1/users/{userId}/categories` | Return inventory categories for a user |
| `GET` | `/v1/users/{userId}/categories/favorites` | Return favorites categories for a user |
| `POST` | `/v1/users/{userId}/challenges/authenticator/verify` | Verifies a two step verification challenge code via authenticator app. |
| `POST` | `/v1/users/{userId}/challenges/cross-device/retract` | Reverts a user's dialog state from ACTIVE to PENDING. |
| `POST` | `/v1/users/{userId}/challenges/cross-device/retry` | Retry a Cross Device two step verification approval. |
| `POST` | `/v1/users/{userId}/challenges/cross-device/verify` | Verifies a two step verification approval via Cross Device. Cross Device approval does not use a ver |
| `POST` | `/v1/users/{userId}/challenges/email/send-code` | Sends a two step verification challenge code via email. |
| `POST` | `/v1/users/{userId}/challenges/email/verify` | Verifies a two step verification challenge with a code sent via email. |
| `POST` | `/v1/users/{userId}/challenges/passkey/verify-finish` | Validates the assertion data returned by the passkey. |
| `POST` | `/v1/users/{userId}/challenges/passkey/verify-start` | Provides a challenge for the passkey to authenticate. |
| `POST` | `/v1/users/{userId}/challenges/password/verify` | Verifies a two step verification challenge with a password (code). |
| `POST` | `/v1/users/{userId}/challenges/recovery-codes/verify` | Verifies a two step verification challenge via a recovery code. |
| `POST` | `/v1/users/{userId}/challenges/security-key/verify-finish` | Validates the assertion data returned by the security key. |
| `POST` | `/v1/users/{userId}/challenges/security-key/verify-start` | Provides a challenge for the security key to authenticate. |
| `POST` | `/v1/users/{userId}/challenges/sms/send-code` | Sends a two step verification code via SMS for the specified user. |
| `POST` | `/v1/users/{userId}/challenges/sms/verify` | Verifies a two step verification challenge with a code sent via SMS. |
| `GET` | `/v1/users/{userId}/configuration` | Gets two step verification configuration for the specified user. |
| `POST` | `/v1/users/{userId}/configuration/authenticator/disable` | Disables two step verification via authenticator for the specified user. |
| `POST` | `/v1/users/{userId}/configuration/authenticator/enable` | Initiates enabling authenticator-based two step verification for the specified user. |
| `POST` | `/v1/users/{userId}/configuration/authenticator/enable-verify` | Finishes enabling authenticator-based two step verification for the specified user. |
| `POST` | `/v1/users/{userId}/configuration/email/disable` | Disables two step verification via email for the specified user. |
| `POST` | `/v1/users/{userId}/configuration/email/enable` | Enables two step verification via email for the specified user. |
| `POST` | `/v1/users/{userId}/configuration/security-key/disable` | Disables a batch of credentials for the specified user. |
| `POST` | `/v1/users/{userId}/configuration/security-key/enable` | Initiates security key registration by providing credential creation options. |
| `POST` | `/v1/users/{userId}/configuration/security-key/enable-verify` | Finishes security key registration and stores credential. Enables security key as a 2sv media type i |
| `POST` | `/v1/users/{userId}/configuration/security-key/list` | List a user's registered security keys. |
| `POST` | `/v1/users/{userId}/configuration/sms/disable` | Disables two step verification via SMS for the specified user. |
| `POST` | `/v1/users/{userId}/configuration/sms/enable` | Enables two step verification via SMS for the specified user. |
| `GET` | `/v1/users/{userId}/currently-wearing` | Gets a list of asset ids that the user is currently wearing. |
| `PATCH` | `/v1/users/{userId}/display-names` | Set the display name for the authorized user. |
| `GET` | `/v1/users/{userId}/display-names/validate` | Validate a display name for an existing user. |
| `GET` | `/v1/users/{userId}/friends` | Get list of all friends for the specified user. |
| `GET` | `/v1/users/{userId}/friends/count` | Get the number of friends a user has |
| `GET` | `/v1/users/{userId}/friends/find` | Get a paginated list of all friends for the specified user. |
| `GET` | `/v1/users/{userId}/friends/groups/roles` | Gets a list of all groups the specified users' friends are in. |
| `GET` | `/v1/users/{userId}/friends/inactive` | Get list of inactive friends for the specified user. |
| `GET` | `/v1/users/{userId}/friends/online` | Get list of all online friends for the specified user. |
| `GET` | `/v1/users/{userId}/friends/search` | Search for friends by name using a text query. |
| `GET` | `/v1/users/{userId}/friends/statuses` | Gets a list of friend statuses of specified users against the specified user. |
| `GET` | `/v1/users/{userId}/groups/primary/role` | Gets a user's primary group. |
| `GET` | `/v1/users/{userId}/groups/roles` | Gets a list of all group roles for groups the specified user is in. |
| `GET` | `/v1/users/{userId}/items/{itemType}/{itemTargetId}` | Gets owned items of the specified item type. Game Servers can make requests for any user, but can on |
| `GET` | `/v1/users/{userId}/items/{itemType}/{itemTargetId}/is-owned` | Gets whether a user owns an item of type itemType with id itemTargetId. |
| `GET` | `/v1/users/{userId}/outfits` | Deprecated, user v2. Gets a list of outfits for the specified user. |
| `GET` | `/v1/users/{userId}/places/inventory` | Gets Created, MyGames, or OtherGames places inventory for a user |
| `GET` | `/v1/users/{userId}/premium-upsell-precheck` | Premium upsell precheck |
| `GET` | `/v1/users/{userId}/promotion-channels` | Get promotion channels for a given user ID |
| `GET` | `/v1/users/{userId}/recovery-codes` | Gets the current status of recovery codes for a user. |
| `POST` | `/v1/users/{userId}/recovery-codes/clear` | Clears any existing recovery codes for the user. |
| `POST` | `/v1/users/{userId}/recovery-codes/regenerate` | Clears any existing recovery codes and generates a new batch of recovery codes. |
| `GET` | `/v1/users/{userId}/roblox-badges` | Returns a list of Roblox badges belonging to a user. |
| `GET` | `/v1/users/{userId}/universes` | Gets all the followings between a user with userId and universes |
| `DELETE` | `/v1/users/{userId}/universes/{universeId}` | Deletes the following between a user with userId and universe with universeId |
| `POST` | `/v1/users/{userId}/universes/{universeId}` | Creates the following between a user with userId and universe with universeId |
| `GET` | `/v1/users/{userId}/universes/{universeId}/status` | Gets the status of a following relationship between a user and a universe. |
| `GET` | `/v1/users/{userId}/username-history` | Retrieves the username history for a particular user. |
| `GET` | `/v1/users/{userId}/validate-membership` | Get if a user has a Premium membership |

### `POST` `/v1/users`

Does not require X-CSRF-Token protection because this is essentially a get request but as a POST to avoid URI limits.

**Request Body:** The Roblox.Users.Api.MultiGetByUserIdRequest.

**Responses:**

- `200` - OK
- `400` - 1: Too many ids.

### `POST` `/v1/users/{targetUserId}/follow`

**Parameters:**

- `targetUserId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: The target user is invalid or does not exist. 6: Invalid parameters. 8: The user cannot follow 
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: The user is banned from performing operation. 3: The user is blocked
- `429` - 9: The flood limit has been exceeded.

### `GET` `/v1/users/{targetUserId}/followers`

**Parameters:**

- `targetUserId` (path, integer (required)) - 
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `400` - 1: The target user is invalid or does not exist. 6: Invalid parameters.
- `403` - 2: The user is banned from performing operation. 3: The user is blocked from performing this action
- `429` - 9: The flood limit has been exceeded.

### `GET` `/v1/users/{targetUserId}/followers/count`

**Parameters:**

- `targetUserId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: The target user is invalid or does not exist.

### `GET` `/v1/users/{targetUserId}/followings`

**Parameters:**

- `targetUserId` (path, integer (required)) - 
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `400` - 1: The target user is invalid or does not exist. 6: Invalid parameters.
- `403` - 2: The user is banned from performing operation. 3: The user is blocked from performing this action
- `429` - 9: The flood limit has been exceeded.

### `GET` `/v1/users/{targetUserId}/followings/count`

**Parameters:**

- `targetUserId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: The target user is invalid or does not exist.

### `POST` `/v1/users/{targetUserId}/unfollow`

**Parameters:**

- `targetUserId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: The target user is invalid or does not exist. 6: Invalid parameters. 8: The user cannot follow 
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: The user is banned from performing operation. 3: The user is blocked
- `429` - 9: The flood limit has been exceeded.

### `GET` `/v1/users/{userId}`

**Parameters:**

- `userId` (path, integer (required)) - The user id.

**Responses:**

- `200` - OK
- `404` - 3: The user id is invalid.

### `GET` `/v1/users/{userId}/assets/collectibles`

**Parameters:**

- `userId` (path, integer (required)) - The userid of the owner of the collectibles.
- `assetType` (query, integer) - The asset type for the collectibles you're trying to get.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - Sorted by userAssetId

**Responses:**

- `200` - OK
- `400` - The specified asset type(s) are invalid.
- `403` - The specified user's inventory is hidden.

### `GET` `/v1/users/{userId}/avatar`

Includes assets, bodycolors, and playerAvatarType.

**Parameters:**

- `userId` (path, integer (required)) - 
- `Roblox-Place-Id` (header, integer) - 

**Responses:**

- `200` - OK
- `400` - 1: The specified user does not exist. 2: An account for the given userId does not exist!

### `GET` `/v1/users/{userId}/badges`

**Parameters:**

- `userId` (path, integer (required)) - The user Id.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `404` - 4: User is invalid or does not exist.

### `GET` `/v1/users/{userId}/badges/awarded-dates`

**Parameters:**

- `userId` (path, integer (required)) - The user Id.
- `badgeIds` (query, array (required)) - The CSV of badge Ids.

**Responses:**

- `200` - OK
- `400` - 5: Too many badge Ids.
- `404` - 4: User is invalid or does not exist.

### `GET` `/v1/users/{userId}/badges/{badgeId}/awarded-date`

**Parameters:**

- `userId` (path, integer (required)) - User id.
- `badgeId` (path, integer (required)) - Badge id.

**Responses:**

- `200` - OK
- `404` - 4: User is invalid or does not exist.

### `GET` `/v1/users/{userId}/bundles`

**Parameters:**

- `userId` (path, integer (required)) - 
- `cursor` (query, string) - 
- `limit` (query, integer) - 
- `sortOrder` (query, integer) - 

**Responses:**

- `200` - OK
- `400` - 1: Invalid bundle

### `GET` `/v1/users/{userId}/bundles/{bundleType}`

**Parameters:**

- `userId` (path, integer (required)) - 
- `bundleType` (path, integer (required)) - 
- `cursor` (query, string (required)) - 
- `limit` (query, integer) - 
- `sortOrder` (query, integer) - 

**Responses:**

- `200` - OK

### `GET` `/v1/users/{userId}/can-trade-with`

**Parameters:**

- `userId` (path, integer (required)) - The other user's id.

**Responses:**

- `200` - OK
- `400` - 10: Invalid trade partner. See field for whether the invalid partner is the sender or receiver.
- `401` - 0: Authorization has been denied for this request.

### `GET` `/v1/users/{userId}/can-view-inventory`

**Parameters:**

- `userId` (path, integer (required)) - The user identifier.

**Responses:**

- `200` - OK
- `400` - 1: The specified user does not exist!

### `GET` `/v1/users/{userId}/categories`

**Parameters:**

- `userId` (path, integer (required)) - 

**Responses:**

- `200` - OK

### `GET` `/v1/users/{userId}/categories/favorites`

**Parameters:**

- `userId` (path, integer (required)) - 

**Responses:**

- `200` - OK

### `POST` `/v1/users/{userId}/challenges/authenticator/verify`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Responses:**

- `200` - OK
- `400` - 1: Invalid challenge ID. 2: The user ID is invalid. 10: The two step verification challenge code i
- `403` - 0: Token Validation Failed
- `429` - 5: Too many requests.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/challenges/cross-device/retract`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Request Body:** The Roblox.TwoStepVerification.Api.RetractDialogRequest.

**Responses:**

- `200` - OK
- `400` - 1: Invalid challenge ID. 2: The user ID is invalid.
- `403` - 0: Token Validation Failed 19: Challenge denied.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/challenges/cross-device/retry`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Request Body:** The Roblox.TwoStepVerification.Api.RetryApprovalRequest.

**Responses:**

- `200` - OK
- `400` - 1: Invalid challenge ID. 2: The user ID is invalid.
- `403` - 0: Token Validation Failed 19: Challenge denied.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/challenges/cross-device/verify`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Request Body:** The Roblox.TwoStepVerification.Api.VerifyApprovalRequest.

**Responses:**

- `200` - OK
- `400` - 0: An unknown error occurred with the request. 1: Invalid challenge ID. 2: The user ID is invalid.
- `403` - 0: Token Validation Failed 19: Challenge denied.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/challenges/email/send-code`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Responses:**

- `200` - OK
- `400` - 1: Invalid challenge ID.
- `403` - 0: Token Validation Failed 2: The user ID is invalid.
- `429` - 5: Too many requests.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/challenges/email/verify`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Responses:**

- `200` - OK
- `400` - 1: Invalid challenge ID. 10: The two step verification challenge code is invalid.
- `403` - 0: Token Validation Failed 2: The user ID is invalid.
- `429` - 5: Too many requests.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/challenges/passkey/verify-finish`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Responses:**

- `200` - OK
- `400` - 1: Invalid challenge ID. 2: The user ID is invalid. 10: The two step verification challenge code i
- `403` - 0: Token Validation Failed
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/challenges/passkey/verify-start`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Responses:**

- `200` - OK
- `400` - 1: Invalid challenge ID. 2: The user ID is invalid.
- `403` - 0: Token Validation Failed 8: The user is not allowed to perform the requested action.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/challenges/password/verify`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Responses:**

- `200` - OK
- `400` - 1: Invalid challenge ID. 4: The password is invalid.
- `403` - 0: Token Validation Failed 2: The user ID is invalid.
- `429` - 5: Too many requests.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/challenges/recovery-codes/verify`

Once a recovery code has been used to verify a challenge it cannot be used again.

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Responses:**

- `200` - OK
- `400` - 1: Invalid challenge ID. 2: The user ID is invalid. 10: The two step verification challenge code i
- `403` - 0: Token Validation Failed
- `429` - 5: Too many requests.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/challenges/security-key/verify-finish`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Responses:**

- `200` - OK
- `400` - 1: Invalid challenge ID. 2: The user ID is invalid. 10: The two step verification challenge code i
- `403` - 0: Token Validation Failed
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/challenges/security-key/verify-start`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Responses:**

- `200` - OK
- `400` - 1: Invalid challenge ID. 2: The user ID is invalid.
- `403` - 0: Token Validation Failed 8: The user is not allowed to perform the requested action.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/challenges/sms/send-code`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Responses:**

- `200` - OK
- `400` - 1: Invalid challenge ID.
- `403` - 0: Token Validation Failed 2: The user ID is invalid.
- `429` - 5: Too many requests.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/challenges/sms/verify`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Responses:**

- `200` - OK
- `400` - 1: Invalid challenge ID. 2: The user ID is invalid. 10: The two step verification challenge code i
- `403` - 0: Token Validation Failed
- `429` - 5: Too many requests.
- `503` - 7: Two step verification is currently under maintenance.

### `GET` `/v1/users/{userId}/configuration`

**Parameters:**

- `userId` (path, integer (required)) - The Id of the user to get the configuration for.
- `challengeId` (query, string) - The active challenge for the user (as an alternative when the user is unauthenticated).
- `actionType` (query, integer) - The action type the challengeId is associated with.

**Responses:**

- `200` - OK
- `400` - 1: Invalid challenge ID.
- `403` - 2: The user ID is invalid.

### `POST` `/v1/users/{userId}/configuration/authenticator/disable`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Responses:**

- `200` - OK
- `400` - 2: The user ID is invalid. 4: The password is invalid.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 8: The user is not allowed to perform the requested action.
- `429` - 5: Too many requests.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/configuration/authenticator/enable`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Request Body:** The Roblox.TwoStepVerification.Api.EnableTwoStepVerificationRequest.

**Responses:**

- `200` - OK
- `400` - 2: The user ID is invalid. 3: The email is invalid. 4: The password is invalid.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 11: The two step verification configuration is already enabled.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/configuration/authenticator/enable-verify`

Enabling authenticator-based two step verification requires two parts to help ensure
the user has properly stored the authenticator key in their authenticator app.

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Request Body:** The Roblox.TwoStepVerification.Api.EnableVerifyAuthenticatorRequest.

**Responses:**

- `200` - OK
- `400` - 2: The user ID is invalid. 4: The password is invalid. 10: The two step verification challenge cod
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 11: The two step verification configuration is already enabled.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/configuration/email/disable`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Responses:**

- `200` - OK
- `400` - 4: The password is invalid.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: The user ID is invalid. 8: The user is not allowed to perform the re
- `429` - 5: Too many requests.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/configuration/email/enable`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Request Body:** The request body.

**Responses:**

- `200` - OK
- `400` - 3: The email is invalid. 4: The password is invalid.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: The user ID is invalid.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/configuration/security-key/disable`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Request Body:** The request bodyRoblox.TwoStepVerification.Api.DisableTwoStepVerificationRequest.

**Responses:**

- `200` - OK
- `400` - 4: The password is invalid.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 8: The user is not allowed to perform the requested action.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/configuration/security-key/enable`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Responses:**

- `200` - OK
- `400` - 2: The user ID is invalid. 4: The password is invalid.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 9: The two step verification configuration is invalid for this action. 
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/configuration/security-key/enable-verify`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Request Body:** The request body.Roblox.TwoStepVerification.Api.EnableVerifySecurityKeyRequest.

**Responses:**

- `200` - OK
- `400` - 2: The user ID is invalid. 17: Invalid security key nickname.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 17: Invalid security key nickname.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/configuration/security-key/list`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Responses:**

- `200` - OK
- `400` - 2: The user ID is invalid.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/configuration/sms/disable`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Request Body:** The request body.Roblox.TwoStepVerification.Api.DisableTwoStepVerificationRequest.

**Responses:**

- `200` - OK
- `400` - 4: The password is invalid.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: The user ID is invalid. 8: The user is not allowed to perform the re
- `429` - 5: Too many requests.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/configuration/sms/enable`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Responses:**

- `200` - OK
- `400` - 4: The password is invalid. 15: The phone number is invalid.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: The user ID is invalid.
- `503` - 7: Two step verification is currently under maintenance. 8: The user is not allowed to perform the 

### `GET` `/v1/users/{userId}/currently-wearing`

**Parameters:**

- `userId` (path, integer (required)) - The user id.
- `Roblox-Place-Id` (header, integer) - 

**Responses:**

- `200` - OK
- `400` - 1: The specified user does not exist. 2: An account for the given userId does not exist!

### `PATCH` `/v1/users/{userId}/display-names`

**Parameters:**

- `userId` (path, integer (required)) - the user id

**Request Body:** Roblox.Users.Api.SetDisplayNameRequest

**Responses:**

- `200` - OK
- `400` - 1: Display name is too short 2: Display name is too long 3: Display name contains invalid characte
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 7: The user id is invalid.
- `429` - 5: Display name updates for this user have been throttled

### `GET` `/v1/users/{userId}/display-names/validate`

**Parameters:**

- `userId` (path, integer (required)) - The user id.
- `displayName` (query, string (required)) - The display name.

**Responses:**

- `200` - OK
- `400` - 1: Display name is too short 2: Display name is too long 3: Display name contains invalid characte
- `401` - 0: Authorization has been denied for this request.
- `403` - 7: The user id is invalid.
- `429` - 5: Display name updates for this user have been throttled

### `GET` `/v1/users/{userId}/friends`

**Parameters:**

- `userId` (path, integer (required)) - The user Id to get the friends for.
- `userSort` (query, integer) - Specifies how to sort the returned friends.

**Responses:**

- `200` - OK
- `400` - 1: The target user is invalid or does not exist.

### `GET` `/v1/users/{userId}/friends/count`

**Parameters:**

- `userId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: The target user is invalid or does not exist.

### `GET` `/v1/users/{userId}/friends/find`

**Parameters:**

- `userId` (path, integer (required)) - The user Id to get the friends for.
- `userSort` (query, integer) - Specifies how to sort the returned friends.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `limit` (query, integer) - The number of results per request.
- `findFriendsType` (query, integer) - 

**Responses:**

- `200` - OK
- `400` - 1: The target user is invalid or does not exist. 6: Invalid parameters.

### `GET` `/v1/users/{userId}/friends/groups/roles`

**Parameters:**

- `userId` (path, integer (required)) - The user id.

**Responses:**

- `200` - OK
- `400` - 3: The user is invalid or does not exist.
- `403` - 3: The user is invalid or does not exist.

### `GET` `/v1/users/{userId}/friends/inactive`

**Parameters:**

- `userId` (path, integer (required)) - The user Id to get the friends for.

**Responses:**

- `200` - OK
- `400` - 1: The target user is invalid or does not exist. 6: Invalid parameters.
- `401` - 0: Authorization has been denied for this request.

### `GET` `/v1/users/{userId}/friends/online`

**Parameters:**

- `userId` (path, integer (required)) - The user Id to get the friends for.
- `userSort` (query, integer) - The sort order to return the friends.

**Responses:**

- `200` - OK
- `400` - 1: The target user is invalid or does not exist. 6: Invalid parameters.
- `401` - 0: Authorization has been denied for this request.

### `GET` `/v1/users/{userId}/friends/search`

**Parameters:**

- `userId` (path, integer (required)) - The user Id to get the friends for.
- `query` (query, string) - The string to search names of friends for.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `limit` (query, integer) - The number of results per request.

**Responses:**

- `200` - OK
- `400` - 1: The target user is invalid or does not exist. 6: Invalid parameters.
- `401` - 0: Authorization has been denied for this request.

### `GET` `/v1/users/{userId}/friends/statuses`

**Parameters:**

- `userId` (path, integer (required)) - The user to check the friend statuses against.
- `userIds` (query, array (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: The target user is invalid or does not exist. 15: Too many ids. 16: Invalid ids.

### `GET` `/v1/users/{userId}/groups/primary/role`

**Parameters:**

- `userId` (path, integer (required)) - The user id.

**Responses:**

- `200` - OK
- `400` - 4: User is invalid or does not exist.

### `GET` `/v1/users/{userId}/groups/roles`

**Parameters:**

- `userId` (path, integer (required)) - The user id.
- `includeLocked` (query, boolean) - 
- `includeNotificationPreferences` (query, boolean) - 
- `discoveryType` (query, integer) - 

**Responses:**

- `200` - OK
- `400` - 3: The user is invalid or does not exist.

### `GET` `/v1/users/{userId}/items/{itemType}/{itemTargetId}`

**Parameters:**

- `userId` (path, integer (required)) - ID of the user in question
- `itemType` (path, integer (required)) - Type of the item in question (i.e. Asset, GamePass, Badge, Bundle)
- `itemTargetId` (path, integer (required)) - ID of the item in question

**Responses:**

- `200` - OK
- `400` - 1: The specified user does not exist! 5: The specified game pass does not exist! Are you using the 

### `GET` `/v1/users/{userId}/items/{itemType}/{itemTargetId}/is-owned`

**Parameters:**

- `userId` (path, integer (required)) - ID of the user in question
- `itemType` (path, integer (required)) - Type of the item in question (i.e. Asset, GamePass, Badge, Bundle)
- `itemTargetId` (path, integer (required)) - ID of the item in question

**Responses:**

- `200` - OK
- `400` - 1: The specified user does not exist! 5: The specified game pass does not exist! Are you using the 

### `GET` `/v1/users/{userId}/outfits`

**Parameters:**

- `userId` (path, integer (required)) - The user id.
- `outfitType` (query, string) - The outfit type being searched for, null will return all outfitTypes.
- `page` (query, integer) - The page number of the current page of requests, default is 1.
- `itemsPerPage` (query, integer) - The max number of outfits that can be returned.
- `isEditable` (query, boolean) - Whether the outfits are editable. A null value will lead to no filtering.
- `Roblox-Place-Id` (header, integer) - The placeId of the caller, not required to be passed in.

**Responses:**

- `200` - OK
- `400` - 1: The specified user does not exist. 2: An account for the given userId does not exist!

### `GET` `/v1/users/{userId}/places/inventory`

**Parameters:**

- `userId` (path, integer (required)) - 
- `placesTab` (query, integer (required)) - 
- `itemsPerPage` (query, integer (required)) - 
- `cursor` (query, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 6: Invalid request
- `403` - 3: Insufficient permission.

### `GET` `/v1/users/{userId}/premium-upsell-precheck`

**Parameters:**

- `userId` (path, integer (required)) - User ID
- `universeId` (query, integer (required)) - 
- `placeId` (query, integer (required)) - 

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

### `GET` `/v1/users/{userId}/promotion-channels`

**Parameters:**

- `userId` (path, integer (required)) - The ID of the user to fetch the promotion channels for.
- `alwaysReturnUrls` (query, boolean) - Whether all promotion channel links should be returned as full URLs.
- `filterLink` (query, boolean) - Whether all promotion channel links should be filtered.

**Responses:**

- `200` - OK
- `400` - 1: User not found.

### `GET` `/v1/users/{userId}/recovery-codes`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Responses:**

- `200` - OK
- `400` - 2: The user ID is invalid.
- `401` - 0: Authorization has been denied for this request.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/recovery-codes/clear`

Clearing recovery codes voids any recovery codes previously generated for the user.
New recovery codes will have to be generated to pass two step verification via recovery code.

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Request Body:** The Roblox.TwoStepVerification.Api.ClearRecoveryCodesRequest.

**Responses:**

- `200` - OK
- `400` - 2: The user ID is invalid. 4: The password is invalid.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `429` - 5: Too many requests.
- `503` - 7: Two step verification is currently under maintenance.

### `POST` `/v1/users/{userId}/recovery-codes/regenerate`

Two step verification recovery codes do not enforce that two step verification must be passed when logging in.
At least one two step verification media type must be enabled to trigger the two step verification flow.
Recovery codes are intended to be used to pass two step verification when the enabled media type is unavailable.

Recovery codes generated by this endpoint do not have an expiration.

Once a recovery code generated by this endpoint has been used it cannot be used again.

**Parameters:**

- `userId` (path, integer (required)) - The user ID to generate recovery codes for.

**Request Body:** The Roblox.TwoStepVerification.Api.RegenerateRecoveryCodesRequest.

**Responses:**

- `200` - OK
- `400` - 2: The user ID is invalid. 4: The password is invalid.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `429` - 5: Too many requests.
- `503` - 7: Two step verification is currently under maintenance.

### `GET` `/v1/users/{userId}/roblox-badges`

**Parameters:**

- `userId` (path, integer (required)) - 

**Responses:**

- `200` - OK

### `GET` `/v1/users/{userId}/universes`

**Parameters:**

- `userId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - User is not authorized for this action.

### `DELETE` `/v1/users/{userId}/universes/{universeId}`

**Parameters:**

- `userId` (path, integer (required)) - 
- `universeId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - User is not authorized for this action. 0: Token Validation Failed

### `POST` `/v1/users/{userId}/universes/{universeId}`

**Parameters:**

- `userId` (path, integer (required)) - 
- `universeId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - The user has reached the limit of number of followed universes.
- `401` - 0: Authorization has been denied for this request.
- `403` - User is not authorized for this action. 0: Token Validation Failed

### `GET` `/v1/users/{userId}/universes/{universeId}/status`

**Parameters:**

- `userId` (path, integer (required)) - 
- `universeId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - User is not authorized for this action.

### `GET` `/v1/users/{userId}/username-history`

**Parameters:**

- `userId` (path, integer (required)) - 
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `400` - 3: The user id is invalid.

### `GET` `/v1/users/{userId}/validate-membership`

**Parameters:**

- `userId` (path, integer (required)) - User ID

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

---
title: V1 / Groups
type: cloud-api
tags: [Bans and blocks, Groups, Universes, Users]
---

# V1 / Groups

Cloud API resource group with 64 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/groups/{groupId}` | Gets group information |
| `GET` | `/v1/groups/{groupId}/audit-log` | Gets the Group's audit log |
| `GET` | `/v1/groups/{groupId}/bans` | Gets the bans for the group |
| `DELETE` | `/v1/groups/{groupId}/bans/{userId}` | Unbans a user from a group |
| `GET` | `/v1/groups/{groupId}/bans/{userId}` | Fetch the group ban of a user from a group |
| `POST` | `/v1/groups/{groupId}/bans/{userId}` | Bans a user from a group |
| `GET` | `/v1/groups/{groupId}/blocked-keywords` | Retrieves a paginated list of blocked keywords for a specific Group. |
| `POST` | `/v1/groups/{groupId}/blocked-keywords` | Adds new blocked keyword(s) to the specified Group. |
| `DELETE` | `/v1/groups/{groupId}/blocked-keywords/{keywordId}` | Deletes a specific blocked keyword from the specified Group. |
| `PATCH` | `/v1/groups/{groupId}/blocked-keywords/{keywordId}` | Updates an existing blocked keyword for the specified Group. |
| `POST` | `/v1/groups/{groupId}/change-owner` | Changes the group owner to another user. |
| `POST` | `/v1/groups/{groupId}/claim-ownership` | Claims ownership of the group as the authenticated user |
| `GET` | `/v1/groups/{groupId}/community-feature-freezes` | Gets the freeze status of the community features for a group. |
| `GET` | `/v1/groups/{groupId}/configuration` | Gets group configuration information |
| `PATCH` | `/v1/groups/{groupId}/description` | Updates the groups description |
| `GET` | `/v1/groups/{groupId}/emotes` | Gets a groups emote sets. |
| `GET` | `/v1/groups/{groupId}/features` | Gets the freeze status of all features and the lock status for a group. |
| `PATCH` | `/v1/groups/{groupId}/features` | Sets the desired status of group features. Currently only removes active freezes for features set t |
| `GET` | `/v1/groups/{groupId}/features/status` | Checks whether a group has ANY feature disabled (includes feature freezes and group lock). Used to  |
| `DELETE` | `/v1/groups/{groupId}/join-requests` | Batch declines group join requests |
| `GET` | `/v1/groups/{groupId}/join-requests` | Gets a page of Group Join Requests for a group. |
| `POST` | `/v1/groups/{groupId}/join-requests` | Batch accepts group join requests |
| `DELETE` | `/v1/groups/{groupId}/join-requests/users/{userId}` | Declines/cancels a group join request. |
| `GET` | `/v1/groups/{groupId}/join-requests/users/{userId}` | Gets a group join request by userId. |
| `POST` | `/v1/groups/{groupId}/join-requests/users/{userId}` | Accepts a group join request. |
| `GET` | `/v1/groups/{groupId}/membership` | Gets group membership information in the context of the authenticated user |
| `PATCH` | `/v1/groups/{groupId}/name` | Updates the group's name. |
| `GET` | `/v1/groups/{groupId}/name-history` | Gets the Group's name change history. |
| `PATCH` | `/v1/groups/{groupId}/notification-preference` | Updates the group's settings |
| `GET` | `/v1/groups/{groupId}/payout-restriction` | Gets a value indicating whether the group can use payout feature |
| `GET` | `/v1/groups/{groupId}/payouts` | Gets a list of the group payout percentages |
| `POST` | `/v1/groups/{groupId}/payouts` | Pays out a user in Robux. |
| `POST` | `/v1/groups/{groupId}/payouts/recurring` | Updates recurring payouts. |
| `GET` | `/v1/groups/{groupId}/relationships/{groupRelationshipType}` | Gets a group's relationships |
| `DELETE` | `/v1/groups/{groupId}/relationships/{groupRelationshipType}/requests` | Batch declines group affiliate requests |
| `GET` | `/v1/groups/{groupId}/relationships/{groupRelationshipType}/requests` | Gets a group's relationship requests |
| `POST` | `/v1/groups/{groupId}/relationships/{groupRelationshipType}/requests` | Batch accepts group affiliate requests |
| `DELETE` | `/v1/groups/{groupId}/relationships/{groupRelationshipType}/requests/{relatedGroupId}` | Declines a group relationship request. |
| `POST` | `/v1/groups/{groupId}/relationships/{groupRelationshipType}/requests/{relatedGroupId}` | Accepts a group relationship request. |
| `DELETE` | `/v1/groups/{groupId}/relationships/{groupRelationshipType}/{relatedGroupId}` | Deletes a group relationship. |
| `POST` | `/v1/groups/{groupId}/relationships/{groupRelationshipType}/{relatedGroupId}` | Create a group relationship. |
| `GET` | `/v1/groups/{groupId}/revenue/summary/{timeFrame}` |  |
| `GET` | `/v1/groups/{groupId}/roles` | Gets a list of the rolesets in a group. |
| `GET` | `/v1/groups/{groupId}/roles/guest/permissions` | Gets the permissions for a group's guest roleset. These can be viewed by all (members and guests) us |
| `GET` | `/v1/groups/{groupId}/roles/permissions` | Gets all permissions for each role |
| `GET` | `/v1/groups/{groupId}/roles/{roleSetId}/permissions` | Gets the permissions for a group's roleset. The authorized user must either be the group owner or th |
| `PATCH` | `/v1/groups/{groupId}/roles/{roleSetId}/permissions` | Updates the permissions for a group's roleset. The authorized user must be the group owner. |
| `GET` | `/v1/groups/{groupId}/roles/{roleSetId}/users` | Gets a list of users in a group for a specific roleset. |
| `POST` | `/v1/groups/{groupId}/rolesets/create` | Creates new group roleset. |
| `DELETE` | `/v1/groups/{groupId}/rolesets/{rolesetId}` | Deletes existing group roleset. |
| `PATCH` | `/v1/groups/{groupId}/rolesets/{rolesetId}` | Updates existing group roleset. |
| `GET` | `/v1/groups/{groupId}/settings` | Gets the Group's settings |
| `PATCH` | `/v1/groups/{groupId}/settings` | Updates the group's settings |
| `GET` | `/v1/groups/{groupId}/social-links` | Get social link data associated with a group |
| `POST` | `/v1/groups/{groupId}/social-links` | Posts a social links |
| `DELETE` | `/v1/groups/{groupId}/social-links/{socialLinkId}` | Deletes a social link |
| `PATCH` | `/v1/groups/{groupId}/social-links/{socialLinkId}` | Updates a social link |
| `GET` | `/v1/groups/{groupId}/universes` | Gets a list of universes for the given group. |
| `GET` | `/v1/groups/{groupId}/users` | Gets a list of users in a group. |
| `POST` | `/v1/groups/{groupId}/users` | Joins a group |
| `DELETE` | `/v1/groups/{groupId}/users/{userId}` | Removes a user from a group |
| `PATCH` | `/v1/groups/{groupId}/users/{userId}` | Updates a users role in a group. |
| `GET` | `/v1/groups/{groupId}/users/{userId}/permissions` | Gets the permissions a user has in a group. Only available to group owner and RCC |
| `GET` | `/v1/groups/{groupId}/wall/posts` | Gets a list of group wall posts. |

### `GET` `/v1/groups/{groupId}`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist.

### `GET` `/v1/groups/{groupId}/audit-log`

**Parameters:**

- `groupId` (path, integer (required)) - The id of the group the user is in.
- `actionType` (query, string) - Filter for specific type of action performed
- `userId` (query, integer) - Filter for specific user id
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist. 8: Invalid or missing pagination parameters
- `401` - 0: Authorization has been denied for this request.
- `403` - 23: Insufficient permissions to complete the request.

### `GET` `/v1/groups/{groupId}/bans`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 19: You have insufficient permissions for this request.
- `404` - 1: The group is invalid or does not exist.
- `405` - 18: The operation is temporarily unavailable. Please try again later.

### `DELETE` `/v1/groups/{groupId}/bans/{userId}`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.
- `userId` (path, integer (required)) - The Id of the user being unbanned.

**Responses:**

- `200` - OK
- `400` - 29: The user is not banned from the group.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 19: You have insufficient permissions for this request.
- `404` - 1: The group is invalid or does not exist.
- `405` - 18: The operation is temporarily unavailable. Please try again later.

### `GET` `/v1/groups/{groupId}/bans/{userId}`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.
- `userId` (path, integer (required)) - The user Id.

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 19: You have insufficient permissions for this request.
- `404` - 1: The group is invalid or does not exist. 3: The user is invalid or does not exist.
- `405` - 18: The operation is temporarily unavailable. Please try again later.

### `POST` `/v1/groups/{groupId}/bans/{userId}`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.
- `userId` (path, integer (required)) - The Id of the user being banned.

**Responses:**

- `200` - OK
- `400` - 28: The user is already banned from the group. 31: You cannot perform this action against the group
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 19: You have insufficient permissions for this request.
- `404` - 1: The group is invalid or does not exist. 3: The user is invalid or does not exist. 3: The user i
- `405` - 18: The operation is temporarily unavailable. Please try again later.

### `GET` `/v1/groups/{groupId}/blocked-keywords`

**Parameters:**

- `groupId` (path, integer (required)) - 
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist. 6: Limit is invalid.
- `401` - 0: Authorization has been denied for this request.
- `403` - 9: User is invalid or does not exist. 10: Insufficient permissions to complete the request.
- `405` - 31: Service is currently unavailable.

### `POST` `/v1/groups/{groupId}/blocked-keywords`

**Parameters:**

- `groupId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist. 2: One or more keywords are invalid. 4: Invalid request. 1
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 8: Insufficient permissions to complete the request. 9: User is invalid
- `405` - 31: Service is currently unavailable.
- `409` - 11: There was a conflict in your request.

### `DELETE` `/v1/groups/{groupId}/blocked-keywords/{keywordId}`

**Parameters:**

- `groupId` (path, integer (required)) - 
- `keywordId` (path, string (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist. 3: KeywordId is invalid. 4: Invalid request.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 9: User is invalid or does not exist. 10: Insufficient permissions to c
- `404` - 7: Not found.
- `405` - 31: Service is currently unavailable.

### `PATCH` `/v1/groups/{groupId}/blocked-keywords/{keywordId}`

**Parameters:**

- `groupId` (path, integer (required)) - 
- `keywordId` (path, string (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist. 3: KeywordId is invalid. 4: Invalid request. 12: The provi
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 8: Insufficient permissions to complete the request. 9: User is invalid
- `404` - 7: Not found.
- `405` - 31: Service is currently unavailable.
- `409` - 11: There was a conflict in your request.

### `POST` `/v1/groups/{groupId}/change-owner`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.

**Request Body:** The request.

**Responses:**

- `200` - OK
- `400` - 1: The group is invalid or does not exist. 3: The user is invalid or does not exist. 15: User is n
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 17: You are not authorized to change the owner of this group. 25: 2-Ste

### `POST` `/v1/groups/{groupId}/claim-ownership`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.

**Responses:**

- `200` - OK
- `400` - 1: The group is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 11: You are not authorized to claim this group 12: This group already h
- `503` - 18: The operation is temporarily unavailable. Please try again later.

### `GET` `/v1/groups/{groupId}/community-feature-freezes`

**Parameters:**

- `groupId` (path, integer (required)) - 

**Responses:**

- `200` - OK

### `GET` `/v1/groups/{groupId}/configuration`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist. 15: User is not a member of the group.
- `403` - 1: Group is invalid or does not exist. 23: Insufficient permissions to complete the request.
- `503` - 31: Service is currently unavailable.

### `PATCH` `/v1/groups/{groupId}/description`

**Parameters:**

- `groupId` (path, integer (required)) - The id of the group the user is in.

**Request Body:** The Roblox.Groups.Api.UpdateGroupDescriptionRequest.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist. 29: Your group description was empty.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: The description is too long. 23: Insufficient permissions to comple

### `GET` `/v1/groups/{groupId}/emotes`

**Parameters:**

- `groupId` (path, integer (required)) - 

**Responses:**

- `200` - OK

### `GET` `/v1/groups/{groupId}/features`

**Parameters:**

- `groupId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 23: Insufficient permissions to complete the request. 49: User is invalid or does not exist

### `PATCH` `/v1/groups/{groupId}/features`

**Parameters:**

- `groupId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 23: Insufficient permissions to complete the request. 49: User is inval

### `GET` `/v1/groups/{groupId}/features/status`

**Parameters:**

- `groupId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 23: Insufficient permissions to complete the request. 49: User is invalid or does not exist

### `DELETE` `/v1/groups/{groupId}/join-requests`

**Parameters:**

- `groupId` (path, integer (required)) - The group id.

**Responses:**

- `200` - OK
- `400` - 1: The group is invalid or does not exist. 3: The user is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

### `GET` `/v1/groups/{groupId}/join-requests`

**Parameters:**

- `groupId` (path, integer (required)) - The group id.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `400` - 1: The group is invalid or does not exist. 36: The pagination cursor is invalid.
- `401` - 0: Authorization has been denied for this request.
- `403` - 19: You have insufficient permissions for this request.

### `POST` `/v1/groups/{groupId}/join-requests`

**Parameters:**

- `groupId` (path, integer (required)) - The group id.

**Responses:**

- `200` - OK
- `400` - 1: The group is invalid or does not exist. 3: The user is invalid or does not exist. 20: The group
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 6: You are already in the maximum number of groups. 19: You have insuff
- `500` - 0: Something went wrong.
- `503` - 18: The operation is temporarily unavailable. Please try again later.

### `DELETE` `/v1/groups/{groupId}/join-requests/users/{userId}`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.
- `userId` (path, integer (required)) - The user Id.

**Responses:**

- `200` - OK
- `400` - 1: The group is invalid or does not exist. 3: The user is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 4: You do not have permission to manage this member.

### `GET` `/v1/groups/{groupId}/join-requests/users/{userId}`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.
- `userId` (path, integer (required)) - The user Id.

**Responses:**

- `200` - OK
- `400` - 1: The group is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 19: You have insufficient permissions for this request.

### `POST` `/v1/groups/{groupId}/join-requests/users/{userId}`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.
- `userId` (path, integer (required)) - The user Id.

**Responses:**

- `200` - OK
- `400` - 1: The group is invalid or does not exist. 3: The user is invalid or does not exist. 20: The group
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 6: You are already in the maximum number of groups. 19: You have insuff
- `503` - 18: The operation is temporarily unavailable. Please try again later.

### `GET` `/v1/groups/{groupId}/membership`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.
- `includeNotificationPreferences` (query, boolean (required)) - 

**Responses:**

- `200` - OK
- `400` - 1: The group is invalid or does not exist.

### `PATCH` `/v1/groups/{groupId}/name`

This endpoint will charge Robux for the group rename.

**Parameters:**

- `groupId` (path, integer (required)) - The id of the group the user is in.

**Request Body:** The Roblox.Groups.Api.UpdateGroupNameRequest.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist. 13: The name is invalid. 19: The name is too long. 20: The
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 12: Insufficient Robux funds. 14: The name is moderated. 23: Insuffici
- `409` - 36: The name was changed too recently. 37: The name was in use too recently.
- `413` - 0: Unknown error.
- `429` - 17: Too many requests.

### `GET` `/v1/groups/{groupId}/name-history`

**Parameters:**

- `groupId` (path, integer (required)) - The id of the group.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist.
- `403` - 23: Insufficient permissions to complete the request.

### `PATCH` `/v1/groups/{groupId}/notification-preference`

**Parameters:**

- `groupId` (path, integer (required)) - The id of the group the user is in.

**Request Body:** Roblox.Groups.Api.UpdateGroupSettingsRequest

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

### `GET` `/v1/groups/{groupId}/payout-restriction`

**Parameters:**

- `groupId` (path, integer (required)) - The group id.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 9: You don't have permission to view this group's payouts.

### `GET` `/v1/groups/{groupId}/payouts`

**Parameters:**

- `groupId` (path, integer (required)) - The group id.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 9: You don't have permission to view this group's payouts.

### `POST` `/v1/groups/{groupId}/payouts`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist. 12: Insufficient Robux funds. 24: Invalid payout type. 25:
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 23: Insufficient permissions to complete the request. 28: Group has pai
- `503` - 22: The feature is disabled.

### `POST` `/v1/groups/{groupId}/payouts/recurring`

This endpoint will remove any recipients not sent in the request.
If a recipient in the request is not a valid member in the group they will not be added to the recurring payouts.

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist. 24: Invalid payout type. 25: The amount is invalid. 26: To
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 12: Insufficient Robux funds. 28: Group has paid out too recently. Plea
- `503` - 22: The feature is disabled.

### `GET` `/v1/groups/{groupId}/relationships/{groupRelationshipType}`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.
- `groupRelationshipType` (path, string (required)) - The group relationship type, enemies or allies.
- `StartRowIndex` (query, integer (required)) - The start index of the page request
- `MaxRows` (query, integer (required)) - The maximum number of rows for the page request, should be at least 1.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist. 4: Group relationship type or request type is invalid. 8: I

### `DELETE` `/v1/groups/{groupId}/relationships/{groupRelationshipType}/requests`

**Parameters:**

- `groupId` (path, integer (required)) - The group id.
- `groupRelationshipType` (path, string (required)) - The type of group relationship being made

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

### `GET` `/v1/groups/{groupId}/relationships/{groupRelationshipType}/requests`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.
- `groupRelationshipType` (path, string (required)) - The group relationship type of the request, only allies are supported.
- `StartRowIndex` (query, integer (required)) - The start index of the page request
- `MaxRows` (query, integer (required)) - The maximum number of rows for the page request, should be at least 1.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist. 4: Group relationship type or request type is invalid. 8: I
- `401` - 0: Authorization has been denied for this request.
- `403` - 5: You don't have permission to manage this group's relationships.

### `POST` `/v1/groups/{groupId}/relationships/{groupRelationshipType}/requests`

**Parameters:**

- `groupId` (path, integer (required)) - The group id.
- `groupRelationshipType` (path, string (required)) - The type of group relationship being made

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

### `DELETE` `/v1/groups/{groupId}/relationships/{groupRelationshipType}/requests/{relatedGroupId}`

**Parameters:**

- `groupId` (path, integer (required)) - The group id.
- `groupRelationshipType` (path, string (required)) - The group relationship type, enemies or allies.
- `relatedGroupId` (path, integer (required)) - The id of the group you want to accept the relationship request with.

**Responses:**

- `200` - OK
- `400` - 1: Group relationship type or request type is invalid. 2: Invalid group. 3: Target group is invali
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 9: Insufficient permissions.

### `POST` `/v1/groups/{groupId}/relationships/{groupRelationshipType}/requests/{relatedGroupId}`

**Parameters:**

- `groupId` (path, integer (required)) - The group id.
- `groupRelationshipType` (path, string (required)) - The group relationship type, enemies or allies, only allies are supported.
- `relatedGroupId` (path, integer (required)) - The id of the group you want to accept the relationship request with.

**Responses:**

- `200` - OK
- `400` - 1: Group relationship type or request type is invalid. 2: Invalid group. 3: Target group is invali
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 9: Insufficient permissions.

### `DELETE` `/v1/groups/{groupId}/relationships/{groupRelationshipType}/{relatedGroupId}`

**Parameters:**

- `groupId` (path, integer (required)) - The group id.
- `groupRelationshipType` (path, string (required)) - The group relationship type, enemies or allies.
- `relatedGroupId` (path, integer (required)) - The id of the group you want to delete the relationship with.

**Responses:**

- `200` - OK
- `400` - 2: Invalid group. 3: Target group is invalid or does not exist. 11: Relationship does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 8: You are blocked from communicating with this user.

### `POST` `/v1/groups/{groupId}/relationships/{groupRelationshipType}/{relatedGroupId}`

**Parameters:**

- `groupId` (path, integer (required)) - The group id.
- `groupRelationshipType` (path, string (required)) - The group relationship type, enemies or allies.
- `relatedGroupId` (path, integer (required)) - The id of the group you want to create a relationship with.

**Responses:**

- `200` - OK
- `400` - 1: Group relationship type or request type is invalid. 2: Invalid group. 3: Target group is invali
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 5: Your group does not allow enemy declarations. 6: Other group does no

### `GET` `/v1/groups/{groupId}/revenue/summary/{timeFrame}`

**Operation:** `RevenueSummary_GetGroupRevenueSummary`

**Parameters:**

- `groupId` (path, integer (required)) - 
- `timeFrame` (path (required)) - 

**Responses:**

- `200` - Success

### `GET` `/v1/groups/{groupId}/roles`

**Parameters:**

- `groupId` (path, integer (required)) - The group id.

**Responses:**

- `200` - OK
- `400` - 1: The group is invalid or does not exist.

### `GET` `/v1/groups/{groupId}/roles/guest/permissions`

**Parameters:**

- `groupId` (path, integer (required)) - The group id.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist.

### `GET` `/v1/groups/{groupId}/roles/permissions`

**Parameters:**

- `groupId` (path, integer (required)) - The group id.

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

### `GET` `/v1/groups/{groupId}/roles/{roleSetId}/permissions`

**Parameters:**

- `groupId` (path, integer (required)) - The group id.
- `roleSetId` (path, integer (required)) - The group's role set id.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist. 2: The roleset is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 3: You are not authorized to view/edit permissions for this role.

### `PATCH` `/v1/groups/{groupId}/roles/{roleSetId}/permissions`

**Parameters:**

- `groupId` (path, integer (required)) - The group's id.
- `roleSetId` (path, integer (required)) - The roleset's id.

**Request Body:** The request.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist. 2: The roleset is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 3: You are not authorized to view/edit permissions for this role. 4: Th

### `GET` `/v1/groups/{groupId}/roles/{roleSetId}/users`

**Parameters:**

- `groupId` (path, integer (required)) - The group id.
- `roleSetId` (path, integer (required)) - The group's role set id.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `400` - 1: The group is invalid or does not exist. 36: The pagination cursor is invalid.
- `403` - 2: The roleset is invalid or does not exist. 35: You do not have permission to view this group's me

### `POST` `/v1/groups/{groupId}/rolesets/create`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.

**Request Body:** The Roblox.Groups.Api.Models.Request.CreateRoleSetRequest.

**Responses:**

- `200` - OK
- `400` - 0: Something went wrong. 3: You do not have enough funds to purchase this role. 5: Role name alrea
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 9: You do not have permissions to perform this action.

### `DELETE` `/v1/groups/{groupId}/rolesets/{rolesetId}`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.
- `rolesetId` (path, integer (required)) - The roleset Id.

**Responses:**

- `200` - OK
- `400` - 10: This group does not exist. 15: This role does not exist. 17: Cannot remove any more roles 18:
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 9: You do not have permissions to perform this action. 16: There are us

### `PATCH` `/v1/groups/{groupId}/rolesets/{rolesetId}`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.
- `rolesetId` (path, integer (required)) - The roleset Id.

**Request Body:** The Roblox.Groups.Api.Models.Request.UpdateRoleSetRequest.

**Responses:**

- `200` - OK
- `400` - 5: Role name already exists. 6: Rank value is out of bounds. 7: The role name is too long. 8: The
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 9: You do not have permissions to perform this action.

### `GET` `/v1/groups/{groupId}/settings`

**Parameters:**

- `groupId` (path, integer (required)) - The id of the group the user is in.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 23: Insufficient permissions to complete the request.

### `PATCH` `/v1/groups/{groupId}/settings`

**Parameters:**

- `groupId` (path, integer (required)) - The id of the group the user is in.

**Request Body:** Roblox.Groups.Api.UpdateGroupSettingsRequest

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 23: Insufficient permissions to complete the request.
- `503` - 31: Service is currently unavailable.

### `GET` `/v1/groups/{groupId}/social-links`

**Parameters:**

- `groupId` (path, integer (required)) - The Id of the game

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 13: Only users who are over thirteen years of age may edit social links.
- `404` - 11: Social links cannot be processed as this time.

### `POST` `/v1/groups/{groupId}/social-links`

**Parameters:**

- `groupId` (path, integer (required)) - The id of the group

**Request Body:** The Roblox.Groups.Api.SocialLinkRequest

**Responses:**

- `200` - OK
- `400` - 3: The social link title is too long. 4: The social link title cannot be empty. 5: The social link
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: You do not have permission to configure this social link.
- `404` - 8: The requested group or social link was not found.
- `503` - 11: Social links cannot be processed as this time.

### `DELETE` `/v1/groups/{groupId}/social-links/{socialLinkId}`

**Parameters:**

- `groupId` (path, integer (required)) - The id of the game you are editing, required for permissions checking
- `socialLinkId` (path, integer (required)) - The id of the social link

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist. 10: The social link is not for a group. 15: The social link
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: You do not have permission to configure this social link. 13: Only u
- `404` - 11: Social links cannot be processed as this time.

### `PATCH` `/v1/groups/{groupId}/social-links/{socialLinkId}`

**Parameters:**

- `groupId` (path, integer (required)) - The id of the universe
- `socialLinkId` (path, integer (required)) - The id of the social link being updated

**Request Body:** The Roblox.Groups.Api.SocialLinkRequest.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist. 3: The social link title is too long. 4: The social link ti
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: You do not have permission to configure this social link.
- `404` - 11: Social links cannot be processed as this time.
- `503` - 11: Social links cannot be processed as this time.

### `GET` `/v1/groups/{groupId}/universes`

**Parameters:**

- `groupId` (path, integer (required)) - The group id.
- `isArchived` (query, boolean) - Whether or not to return archived games.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - Sorted by universeId

**Responses:**

- `200` - OK
- `400` - Invalid groupId.

### `GET` `/v1/groups/{groupId}/users`

**Parameters:**

- `groupId` (path, integer (required)) - The group id.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - The order the results are sorted in.

**Responses:**

- `200` - OK
- `400` - 1: The group is invalid or does not exist. 36: The pagination cursor is invalid.
- `403` - 35: You do not have permission to view this group's member list.

### `POST` `/v1/groups/{groupId}/users`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.
- `Roblox-Place-Id` (header, integer) - The place ID of the experience the player is in.
- `Roblox-Game-Id` (header, string) - The player's current game Id.
- `Roblox-Session-Id` (header, string) - The player's current session Id.

**Request Body:** Only supplied when captcha has been solved.

**Responses:**

- `200` - OK
- `400` - 1: The group is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 6: You are already in the maximum number of groups. 9: You do not have 
- `409` - 7: You have already requested to join this group. 8: You are already a member of this group.
- `429` - 10: Too many attempts to join the group. Please try again later.
- `503` - 18: The operation is temporarily unavailable. Please try again later.

### `DELETE` `/v1/groups/{groupId}/users/{userId}`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.
- `userId` (path, integer (required)) - The Id of the user being removed.

**Responses:**

- `200` - OK
- `400` - 1: The group is invalid or does not exist. 3: The user is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 4: You do not have permission to manage this member. 25: 2-Step Verific
- `503` - 18: The operation is temporarily unavailable. Please try again later.

### `PATCH` `/v1/groups/{groupId}/users/{userId}`

**Parameters:**

- `groupId` (path, integer (required)) - The id of the group the user is in.
- `userId` (path, integer (required)) - The id of the user being updated.

**Request Body:** The Roblox.Groups.Api.UpdateUserRoleRequest.

**Responses:**

- `200` - OK
- `400` - 1: The group is invalid or does not exist. 2: The roleset is invalid or does not exist. 3: The use
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 4: You do not have permission to manage this member.
- `503` - 18: The operation is temporarily unavailable. Please try again later.

### `GET` `/v1/groups/{groupId}/users/{userId}/permissions`

**Parameters:**

- `groupId` (path, integer (required)) - The group id.
- `userId` (path, integer (required)) - The user id.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist.
- `403` - 3: You are not authorized to view/edit permissions for this role.
- `404` - 3: The user is invalid or does not exist.

### `GET` `/v1/groups/{groupId}/wall/posts`

**Parameters:**

- `groupId` (path, integer (required)) - The group id.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - Sorted by group wall post Id

**Responses:**

- `200` - OK
- `400` - 1: The group is invalid or does not exist.
- `403` - 2: You do not have permission to access this group wall.

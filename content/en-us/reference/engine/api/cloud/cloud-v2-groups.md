---
title: Cloud / V2 / Groups
type: cloud-api
tags: [Groups]
---

# Cloud / V2 / Groups

Cloud API resource group with 13 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/cloud/v2/groups/{group_id}` | Get Group [BETA] |
| `GET` | `/cloud/v2/groups/{group_id}/forum-categories` | List Group Forum Categories [BETA] |
| `GET` | `/cloud/v2/groups/{group_id}/forum-categories/{forum_category_id}/posts` | List Group Forum Posts [BETA] |
| `GET` | `/cloud/v2/groups/{group_id}/forum-categories/{forum_category_id}/posts/{post_id}/comments` | List Group Forum Comments [BETA] |
| `GET` | `/cloud/v2/groups/{group_id}/join-requests` | List Group Join Requests [BETA] |
| `POST` | `/cloud/v2/groups/{group_id}/join-requests/{join_request_id}:accept` | Accept Group Join Request [BETA] |
| `POST` | `/cloud/v2/groups/{group_id}/join-requests/{join_request_id}:decline` | Decline Group Join Request [BETA] |
| `GET` | `/cloud/v2/groups/{group_id}/memberships` | List Group Memberships [BETA] |
| `PATCH` | `/cloud/v2/groups/{group_id}/memberships/{membership_id}` | Update Group Membership [BETA] |
| `POST` | `/cloud/v2/groups/{group_id}/memberships/{membership_id}:assignRole` | Assign Role Group Membership [BETA] |
| `POST` | `/cloud/v2/groups/{group_id}/memberships/{membership_id}:unassignRole` | Unassign Role Group Membership [BETA] |
| `GET` | `/cloud/v2/groups/{group_id}/roles` | List Group Roles [BETA] |
| `GET` | `/cloud/v2/groups/{group_id}/roles/{role_id}` | Get Group Role [BETA] |

### `GET` `/cloud/v2/groups/{group_id}`

**Operation:** `Cloud_GetGroup`

**Stability:** BETA

Gets the specified group.

**Parameters:**

- `group_id` (path, string (required)) - The group ID.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/groups/{group_id}/forum-categories`

**Operation:** `Cloud_ListGroupForumCategories`

**Stability:** BETA

Lists forum categories in the group. Supports filtering.

**Parameters:**

- `group_id` (path, string (required)) - The group ID.
- `maxPageSize` (query, integer) - The maximum number of group forum categories to return. The service might return fewer than this value. If unspecified, at most 10 group forum categor
- `pageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page.  When paginating, all other parameters provided to the subsequent call mus
- `filter` (query, string) - This field may be set in order to filter the resources returned.  Filtering conforms to Common Expression Language (CEL). Only the boolean field `arch

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/groups/{group_id}/forum-categories/{forum_category_id}/posts`

**Operation:** `Cloud_ListGroupForumPosts`

**Stability:** BETA

Lists forum posts in the group's forum category. Supports filtering.

**Parameters:**

- `group_id` (path, string (required)) - The group ID.
- `forum_category_id` (path, string (required)) - The forum-category ID.
- `maxPageSize` (query, integer) - The maximum number of group forum posts to return. The service might return fewer than this value. If unspecified, at most 10 group forum posts are re
- `pageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page.  When paginating, all other parameters provided to the subsequent call mus
- `filter` (query, string) - This field may be set in order to filter the resources returned.  Filtering conforms to Common Expression Language (CEL). Only the query `filter=pinne
- `view` (query, string) - The view in which to retrieve the group forum post.  Supports FULL and FULL_WITH_FIRST_COMMENT.  Defaults to FULL.  Possible values:    | Value | Desc

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/groups/{group_id}/forum-categories/{forum_category_id}/posts/{post_id}/comments`

**Operation:** `Cloud_ListGroupForumComments`

**Stability:** BETA

Lists forum comments on a group's forum post. Supports filtering.

**Parameters:**

- `group_id` (path, string (required)) - The group ID.
- `forum_category_id` (path, string (required)) - The forum-category ID.
- `post_id` (path, string (required)) - The post ID.
- `maxPageSize` (query, integer) - The maximum number of group forum comments to return. The service might return fewer than this value. If unspecified, at most 10 group forum comments 
- `pageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page.  When paginating, all other parameters provided to the subsequent call mus
- `filter` (query, string) - This field may be set in order to filter the resources returned.  Filtering conforms to Common Expression Language (CEL). Only the string field `repli

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/groups/{group_id}/join-requests`

**Operation:** `Cloud_ListGroupJoinRequests`

**Stability:** BETA

List join requests under a group. Supports filtering.

**Parameters:**

- `group_id` (path, string (required)) - The group ID.
- `maxPageSize` (query, integer) - The maximum number of group join requests to return. The service might return fewer than this value. If unspecified, at most 10 group join requests ar
- `pageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page.  When paginating, all other parameters provided to the subsequent call mus
- `filter` (query, string) - This field may be set in order to filter the resources returned.  Filtering conforms to Common Expression Language (CEL). Only the `user` field and `=

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/groups/{group_id}/join-requests/{join_request_id}:accept`

**Operation:** `Cloud_AcceptGroupJoinRequest`

**Stability:** BETA

Accepts a join request.

**Parameters:**

- `group_id` (path, string (required)) - The group ID.
- `join_request_id` (path, string (required)) - The join-request ID.

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/groups/{group_id}/join-requests/{join_request_id}:decline`

**Operation:** `Cloud_DeclineGroupJoinRequest`

**Stability:** BETA

Declines a join request.

**Parameters:**

- `group_id` (path, string (required)) - The group ID.
- `join_request_id` (path, string (required)) - The join-request ID.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/groups/{group_id}/memberships`

**Operation:** `Cloud_ListGroupMemberships`

**Stability:** BETA

List group members in a group. Supports filtering.

**Parameters:**

- `group_id` (path, string (required)) - The group ID.
- `maxPageSize` (query, integer) - The maximum number of group memberships to return. The service might return fewer than this value. If unspecified, at most 10 group memberships are re
- `pageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page.  When paginating, all other parameters provided to the subsequent call mus
- `filter` (query, string) - This field may be set in order to filter the resources returned.  See the [filtering](/cloud/reference/patterns#list-group-memberships) documentation 

**Responses:**

- `200` - OK

### `PATCH` `/cloud/v2/groups/{group_id}/memberships/{membership_id}`

**Operation:** `Cloud_UpdateGroupMembership`

**Stability:** BETA

**Deprecated.** Use AssignGroupRole and UnassignGroupRole instead.
Updates the group membership for a particular group member. This action
requires the requester to be able to manage lower ranked members. Guest or
Owner ranks cannot be assigned, and a requester cannot change their own
rank.

**Parameters:**

- `group_id` (path, string (required)) - The group ID.
- `membership_id` (path, string (required)) - The membership ID.

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/groups/{group_id}/memberships/{membership_id}:assignRole`

**Operation:** `Cloud_AssignRoleGroupMembership`

**Stability:** BETA

Assigns a specific role to a user within a group. If the user already
holds the specified role, no action is taken.

**Parameters:**

- `group_id` (path, string (required)) - The group ID.
- `membership_id` (path, string (required)) - The membership ID.

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/groups/{group_id}/memberships/{membership_id}:unassignRole`

**Operation:** `Cloud_UnassignRoleGroupMembership`

**Stability:** BETA

Unassigns a specific role from a user within a group. If the user does
not hold the specified role, no action is taken.

**Parameters:**

- `group_id` (path, string (required)) - The group ID.
- `membership_id` (path, string (required)) - The membership ID.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/groups/{group_id}/roles`

**Operation:** `Cloud_ListGroupRoles`

**Stability:** BETA

List roles in a group.

The permissions field for roles is viewable based on the requester's access
and scopes.

Permissions for the guest role are always visible - a scope is not needed.

If the requester is a member of the group and has the `group:read` scope,
permissions in their role are visible.

If the requester is the owner of the group and has the `group:read` scope,
permissions in all roles are visible.

**Parameters:**

- `group_id` (path, string (required)) - The group ID.
- `maxPageSize` (query, integer) - The maximum number of group roles to return. The service might return fewer than this value. If unspecified, at most 10 group roles are returned. The 
- `pageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page.  When paginating, all other parameters provided to the subsequent call mus

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/groups/{group_id}/roles/{role_id}`

**Operation:** `Cloud_GetGroupRole`

**Stability:** BETA

Get the group role

**Parameters:**

- `group_id` (path, string (required)) - The group ID.
- `role_id` (path, string (required)) - The role ID.

**Responses:**

- `200` - OK

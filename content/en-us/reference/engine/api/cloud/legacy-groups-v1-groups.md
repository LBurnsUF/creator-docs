---
title: Legacy Groups / V1 / Groups
type: cloud-api
tags: [Groups]
---

# Legacy Groups / V1 / Groups

Cloud API resource group with 7 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/legacy-groups/v1/groups/policies` | Gets group policy info used for compliance. |
| `GET` | `/legacy-groups/v1/groups/{groupId}/audit-log` | Gets the Group's audit log |
| `PATCH` | `/legacy-groups/v1/groups/{groupId}/description` | Updates the groups description |
| `PATCH` | `/legacy-groups/v1/groups/{groupId}/notification-preference` | Updates the group's settings |
| `GET` | `/legacy-groups/v1/groups/{groupId}/settings` | Gets the Group's settings |
| `PATCH` | `/legacy-groups/v1/groups/{groupId}/settings` | Updates the group's settings |
| `PATCH` | `/legacy-groups/v1/groups/{groupId}/status` | Sets group status |

### `POST` `/legacy-groups/v1/groups/policies`

**Responses:**

- `200` - OK
- `400` - 1: Too many ids in request. 2: Ids could not be parsed from request.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

### `GET` `/legacy-groups/v1/groups/{groupId}/audit-log`

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

### `PATCH` `/legacy-groups/v1/groups/{groupId}/description`

**Parameters:**

- `groupId` (path, integer (required)) - The id of the group the user is in.

**Request Body:** The Roblox.Groups.Api.UpdateGroupDescriptionRequest.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist. 29: Your group description was empty.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: The description is too long. 23: Insufficient permissions to comple

### `PATCH` `/legacy-groups/v1/groups/{groupId}/notification-preference`

**Parameters:**

- `groupId` (path, integer (required)) - The id of the group the user is in.

**Request Body:** Roblox.Groups.Api.UpdateGroupSettingsRequest

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

### `GET` `/legacy-groups/v1/groups/{groupId}/settings`

**Parameters:**

- `groupId` (path, integer (required)) - The id of the group the user is in.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 23: Insufficient permissions to complete the request.

### `PATCH` `/legacy-groups/v1/groups/{groupId}/settings`

**Parameters:**

- `groupId` (path, integer (required)) - The id of the group the user is in.

**Request Body:** Roblox.Groups.Api.UpdateGroupSettingsRequest

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 23: Insufficient permissions to complete the request.
- `503` - 31: Service is currently unavailable.

### `PATCH` `/legacy-groups/v1/groups/{groupId}/status`

**Parameters:**

- `groupId` (path, integer (required)) - The group Id.

**Request Body:** The Roblox.Groups.Api.PostGroupStatusRequest.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist. 7: Missing group status content. 32: Description was filter
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 6: You are not authorized to set the status of this group

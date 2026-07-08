---
title: V1 / User / Groups
type: cloud-api
tags: [Assets, Groups, Universes, User profiles, Users]
---

# V1 / User / Groups

Cloud API resource group with 5 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/user/groups/canmanage` | Gets a list of Groups that a user can manage. |
| `GET` | `/v1/user/groups/canmanagegamesoritems` | Gets a list of groups a user can manage games or items for. |
| `GET` | `/v1/user/groups/pending` | Gets groups that the authenticated user has requested to join |
| `DELETE` | `/v1/user/groups/primary` | Removes the authenticated user's primary group |
| `POST` | `/v1/user/groups/primary` | Sets the authenticated user's primary group |

### `GET` `/v1/user/groups/canmanage`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

### `GET` `/v1/user/groups/canmanagegamesoritems`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

### `GET` `/v1/user/groups/pending`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

### `DELETE` `/v1/user/groups/primary`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

### `POST` `/v1/user/groups/primary`

**Request Body:** The request body containing the group id.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: You aren't a member of the group specified.

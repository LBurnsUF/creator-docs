---
title: Legacy Followings / V2 / Users
type: cloud-api
tags: [Interactions, Universes, Users]
---

# Legacy Followings / V2 / Users

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/legacy-followings/v2/users/{userId}/universes` | Gets all universes followed by a user. |

### `GET` `/legacy-followings/v2/users/{userId}/universes`

**Parameters:**

- `userId` (path, integer (required)) - The user ID.

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - User is not authorized for this action.

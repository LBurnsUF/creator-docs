---
title: Legacy Followings / V1 / Users
type: cloud-api
tags: [Interactions, Universes, Users]
---

# Legacy Followings / V1 / Users

Cloud API resource group with 4 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/legacy-followings/v1/users/{userId}/universes` | Gets all the followings between a user with userId and universes |
| `DELETE` | `/legacy-followings/v1/users/{userId}/universes/{universeId}` | Deletes the following between a user with userId and universe with universeId |
| `POST` | `/legacy-followings/v1/users/{userId}/universes/{universeId}` | Creates the following between a user with userId and universe with universeId |
| `GET` | `/legacy-followings/v1/users/{userId}/universes/{universeId}/status` | Gets the status of a following relationship between a user and a universe. |

### `GET` `/legacy-followings/v1/users/{userId}/universes`

**Parameters:**

- `userId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - User is not authorized for this action.

### `DELETE` `/legacy-followings/v1/users/{userId}/universes/{universeId}`

**Parameters:**

- `userId` (path, integer (required)) - 
- `universeId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - User is not authorized for this action. 0: Token Validation Failed

### `POST` `/legacy-followings/v1/users/{userId}/universes/{universeId}`

**Parameters:**

- `userId` (path, integer (required)) - 
- `universeId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - The user has reached the limit of number of followed universes.
- `401` - 0: Authorization has been denied for this request.
- `403` - User is not authorized for this action. 0: Token Validation Failed

### `GET` `/legacy-followings/v1/users/{userId}/universes/{universeId}/status`

**Parameters:**

- `userId` (path, integer (required)) - 
- `universeId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - User is not authorized for this action.

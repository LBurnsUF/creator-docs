---
title: V1 / User / Following Exists
type: cloud-api
tags: [Interactions]
---

# V1 / User / Following Exists

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/user/following-exists` | Returns whether or not the current user is following each userId in a list of userIds |

### `POST` `/v1/user/following-exists`

**Request Body:** The userIds potentially being followed

**Responses:**

- `200` - OK
- `400` - 0: An invalid userId was passed in.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `503` - 1: Followers are disabled at this time.

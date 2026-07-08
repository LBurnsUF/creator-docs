---
title: V1 / User / Tag
type: cloud-api
tags: [Users]
---

# V1 / User / Tag

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/user/tag` | Sets the tag for a user |
| `GET` | `/v1/user/tag/validate` | Validates the tag for a user |

### `POST` `/v1/user/tag`

**Request Body:** The tag receiving userId and the tag itself

**Responses:**

- `200` - OK
- `400` - 2: The target user is invalid or does not exist. 4: Invalid parameters. 6: The userTag is too long
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 5: The user cannot tag themselves.
- `429` - 10: The flood limit has been exceeded.

### `GET` `/v1/user/tag/validate`

**Parameters:**

- `alias` (query, string) - The tag to validate

**Responses:**

- `200` - OK
- `400` - 4: Invalid parameters.
- `401` - 0: Authorization has been denied for this request.
- `429` - 10: The flood limit has been exceeded.

---
title: V1 / User / Badges
type: cloud-api
tags: [Badges]
---

# V1 / User / Badges

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `DELETE` | `/v1/user/badges/{badgeId}` | Removes a badge from the authenticated user. |

### `DELETE` `/v1/user/badges/{badgeId}`

**Parameters:**

- `badgeId` (path, integer (required)) - The badge Id.

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `404` - 1: Badge is invalid or does not exist.

---
title: Legacy Badges / V1 / Badges
type: cloud-api
tags: [Badges]
---

# Legacy Badges / V1 / Badges

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `PATCH` | `/legacy-badges/v1/badges/{badgeId}` | Updates badge configuration. |

### `PATCH` `/legacy-badges/v1/badges/{badgeId}`

**Parameters:**

- `badgeId` (path, integer (required)) - The badge Id.

**Request Body:** The request body.

**Responses:**

- `200` - OK
- `400` - 6: Text moderated. 14: Invalid badge name. 15: Invalid badge description.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: You do not have permission to manage this badge.
- `404` - 1: Badge is invalid or does not exist. 3: The game is invalid or does not exist.

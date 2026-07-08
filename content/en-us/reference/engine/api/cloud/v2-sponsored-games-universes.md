---
title: V2 / Sponsored Games / Universes
type: cloud-api
tags: [Sponsored campaigns]
---

# V2 / Sponsored Games / Universes

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/sponsored-games/universes` | Gets a list of universes for the authenticated user, or the given group, ordered by most recently cr |

### `GET` `/v2/sponsored-games/universes`

**Parameters:**

- `groupId` (query, integer) - The group id, if applicable.

**Responses:**

- `200` - OK
- `400` - 19: Invalid group id.
- `401` - 0: Authorization has been denied for this request.
- `403` - 10: Insufficient permissions.

---
title: Legacy Badges / V1 / Universes
type: cloud-api
tags: [Badges, Universes]
---

# Legacy Badges / V1 / Universes

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/legacy-badges/v1/universes/{universeId}/badges` | Creates a new badge. |

### `POST` `/legacy-badges/v1/universes/{universeId}/badges`

**Parameters:**

- `universeId` (path, integer (required)) - The ID of the universe to create the badge for.

**Responses:**

- `200` - OK
- `400` - 11: The badge icon is invalid. 14: Invalid badge name. 15: Invalid badge description. 16: Payment
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 6: Text moderated. 12: You do not have permission to manage this game's
- `404` - 3: The game is invalid or does not exist.
- `429` - 13: Too many requests, try again later.

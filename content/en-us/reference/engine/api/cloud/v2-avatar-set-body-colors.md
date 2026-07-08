---
title: V2 / Avatar / Set Body Colors
type: cloud-api
tags: [Avatars]
---

# V2 / Avatar / Set Body Colors

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v2/avatar/set-body-colors` | Sets the authenticated user's body colors. |

### `POST` `/v2/avatar/set-body-colors`

**Parameters:**

- `Roblox-Place-Id` (header, integer) - 

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

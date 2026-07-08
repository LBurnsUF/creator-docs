---
title: V1 / Avatar / Set Scales
type: cloud-api
tags: [Avatars]
---

# V1 / Avatar / Set Scales

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/avatar/set-scales` | Sets the authenticated user's scales. |

### `POST` `/v1/avatar/set-scales`

**Parameters:**

- `Roblox-Place-Id` (header, integer) - 

**Responses:**

- `200` - OK
- `400` - 1: Please pass in the scales JSON
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 3: The user does not have permissions to change scales.

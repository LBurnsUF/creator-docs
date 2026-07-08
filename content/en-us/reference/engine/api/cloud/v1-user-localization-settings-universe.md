---
title: V1 / User Localization Settings / Universe
type: cloud-api
tags: [Localization, Universes]
---

# V1 / User Localization Settings / Universe

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/user-localization-settings/universe/{universeId}` | Get user localization settings for universe. |
| `POST` | `/v1/user-localization-settings/universe/{universeId}` | Set user localization settings for universe. |

### `GET` `/v1/user-localization-settings/universe/{universeId}`

**Parameters:**

- `universeId` (path, integer (required)) - The universe's ID.

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id 21: The language is not supported 22: Invalid language code
- `401` - 0: Authorization has been denied for this request.
- `503` - 17: Feature is disabled

### `POST` `/v1/user-localization-settings/universe/{universeId}`

**Parameters:**

- `universeId` (path, integer (required)) - The universe's ID.

**Request Body:** The request body

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id 22: Invalid language code
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `503` - 17: Feature is disabled

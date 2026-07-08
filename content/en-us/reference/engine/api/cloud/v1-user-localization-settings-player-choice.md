---
title: V1 / User Localization Settings / Player Choice
type: cloud-api
tags: [Localization]
---

# V1 / User Localization Settings / Player Choice

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/user-localization-settings/player-choice/{universeId}` | Get user player choice settings for universe. |

### `GET` `/v1/user-localization-settings/player-choice/{universeId}`

**Parameters:**

- `universeId` (path, integer (required)) - The universe's ID.

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id
- `401` - 0: Authorization has been denied for this request.
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

---
title: V1 / Locales / Set Show Roblox Translations
type: cloud-api
tags: [Localization]
---

# V1 / Locales / Set Show Roblox Translations

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/locales/set-show-roblox-translations` | Sets whether translations suggested by Roblox will be shown to the user. |

### `POST` `/v1/locales/set-show-roblox-translations`

**Request Body:** Whether to show Roblox-suggested translations

**Responses:**

- `200` - OK
- `400` - Bad Request
- `401` - Unauthorized 0: Authorization has been denied for this request.
- `403` - Feature is turned off temporary 0: Token Validation Failed
- `500` - Internal server error

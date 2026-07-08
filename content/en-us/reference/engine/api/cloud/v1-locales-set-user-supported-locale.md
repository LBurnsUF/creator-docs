---
title: V1 / Locales / Set User Supported Locale
type: cloud-api
tags: [Localization, Metadata]
---

# V1 / Locales / Set User Supported Locale

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/locales/set-user-supported-locale` | Sets user's supported locale. Null supported locale will clear out user's supported locale (set use |

### `POST` `/v1/locales/set-user-supported-locale`

**Request Body:** Supported locale code that needs to be set for user

**Responses:**

- `200` - OK
- `400` - Bad Request
- `401` - Unauthorized 0: Authorization has been denied for this request.
- `403` - Feature is turned off temporary 0: Token Validation Failed
- `500` - Internal server error

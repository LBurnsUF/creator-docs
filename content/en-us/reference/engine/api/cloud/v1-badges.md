---
title: V1 / Badges
type: cloud-api
tags: [Assets, Badges, Localization, Thumbnails]
---

# V1 / Badges

Cloud API resource group with 12 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/badges/{badgeId}` | Gets badge information by the badge Id. |
| `PATCH` | `/v1/badges/{badgeId}` | Updates badge configuration. |
| `PATCH` | `/v1/badges/{badgeId}/description/language-codes/{languageCode}` | Update localized description of a badge |
| `POST` | `/v1/badges/{badgeId}/icon` | Overwrites a badge icon with a new one. |
| `POST` | `/v1/badges/{badgeId}/icon#PublishApi` | Overwrites a badge icon with a new one. |
| `GET` | `/v1/badges/{badgeId}/icons` | Get all icons for a badge |
| `DELETE` | `/v1/badges/{badgeId}/icons/language-codes/{languageCode}` | Delete a localized icon from a badge |
| `POST` | `/v1/badges/{badgeId}/icons/language-codes/{languageCode}` | Update a badge's icon |
| `GET` | `/v1/badges/{badgeId}/name-description` |  |
| `DELETE` | `/v1/badges/{badgeId}/name-description/language-codes/{languageCode}` | Delete localized name and description of a badge |
| `PATCH` | `/v1/badges/{badgeId}/name-description/language-codes/{languageCode}` | Update localized name and description of a badge |
| `PATCH` | `/v1/badges/{badgeId}/name/language-codes/{languageCode}` | Update localized name of a badge |

### `GET` `/v1/badges/{badgeId}`

**Parameters:**

- `badgeId` (path, integer (required)) - The badge Id.

**Responses:**

- `200` - OK
- `404` - 1: Badge is invalid or does not exist. 3: The game is invalid or does not exist.

### `PATCH` `/v1/badges/{badgeId}`

**Parameters:**

- `badgeId` (path, integer (required)) - The badge Id.

**Request Body:** The request body.

**Responses:**

- `200` - OK
- `400` - 6: Text moderated. 14: Invalid badge name. 15: Invalid badge description.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: You do not have permission to manage this badge.
- `404` - 1: Badge is invalid or does not exist. 3: The game is invalid or does not exist.

### `PATCH` `/v1/badges/{badgeId}/description/language-codes/{languageCode}`

**Parameters:**

- `badgeId` (path, integer (required)) - The badge id
- `languageCode` (path, string (required)) - The language code of the description to update

**Request Body:** The request

**Responses:**

- `200` - OK
- `400` - 13: Request body can't be null 19: New name is null or whitespaces or new name/description is too l
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

### `POST` `/v1/badges/{badgeId}/icon`

**Parameters:**

- `badgeId` (path, integer (required)) - The badge Id.

**Responses:**

- `200` - OK
- `400` - 6: Text moderated. 22: Icon file is not present in the request.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: You do not have permission to manage this badge.
- `404` - 1: Badge is invalid or does not exist.
- `429` - 13: Too many requests, try again later.

### `POST` `/v1/badges/{badgeId}/icon#PublishApi`

**Parameters:**

- `badgeId` (path, integer (required)) - The badge Id.

**Responses:**

- `200` - OK
- `400` - 2: File not present in request. 12: Name or description is moderated.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 5: You do not have permission to manage this item.
- `404` - 4: Target item is invalid or does not exist.
- `429` - 3: You're uploading too much, please wait and try again later.

### `GET` `/v1/badges/{badgeId}/icons`

**Parameters:**

- `badgeId` (path, integer (required)) - The id of the badge
- `width` (query, integer) - The width of the icon to request
- `height` (query, integer) - The height of the icon to request

**Responses:**

- `200` - OK
- `400` - 52: Image dimensions are invalid 62: Invalid game badge id
- `401` - 0: Authorization has been denied for this request.
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

### `DELETE` `/v1/badges/{badgeId}/icons/language-codes/{languageCode}`

**Parameters:**

- `badgeId` (path, integer (required)) - The id of the badge
- `languageCode` (path, string (required)) - The language code of the localized icon to delete

**Responses:**

- `200` - OK
- `400` - 22: Invalid language code 23: You can't delete translations for source language 53: Language is no
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

### `POST` `/v1/badges/{badgeId}/icons/language-codes/{languageCode}`

**Parameters:**

- `badgeId` (path, integer (required)) - The id of the badge
- `languageCode` (path, string (required)) - The language code of this icon to update

**Responses:**

- `200` - OK
- `400` - 22: Invalid language code 26: You can't update translations for source language 45: File uploaded 
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `429` - 24: Too many attempts.Please try again later.
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

### `GET` `/v1/badges/{badgeId}/name-description`

**Parameters:**

- `badgeId` (path, integer (required)) - 

**Responses:**

- `200` - OK
- `400` - 62: Invalid game badge id
- `401` - 0: Authorization has been denied for this request.
- `503` - 17: Feature is disabled

### `DELETE` `/v1/badges/{badgeId}/name-description/language-codes/{languageCode}`

**Parameters:**

- `badgeId` (path, integer (required)) - The badge id
- `languageCode` (path, string (required)) - The language code of the name and description to delete

**Responses:**

- `200` - OK
- `400` - 22: Invalid language code 23: You can't delete translations for source language 53: Language is no
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

### `PATCH` `/v1/badges/{badgeId}/name-description/language-codes/{languageCode}`

**Parameters:**

- `badgeId` (path, integer (required)) - The badge id
- `languageCode` (path, string (required)) - The language code of the name and description to Update

**Request Body:** The request

**Responses:**

- `200` - OK
- `400` - 13: Request body can't be null 19: New name is null or whitespaces or new name/description is too l
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

### `PATCH` `/v1/badges/{badgeId}/name/language-codes/{languageCode}`

**Parameters:**

- `badgeId` (path, integer (required)) - The badge id
- `languageCode` (path, string (required)) - The language code of the name to update

**Request Body:** The request

**Responses:**

- `200` - OK
- `400` - 13: Request body can't be null 19: New name is null or whitespaces or new name/description is too l
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

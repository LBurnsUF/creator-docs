---
title: Legacy Game Internationalization / V1 / Developer Products
type: cloud-api
tags: [Developer products, Localization]
---

# Legacy Game Internationalization / V1 / Developer Products

Cloud API resource group with 8 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `PATCH` | `/legacy-game-internationalization/v1/developer-products/{developerProductId}/description/language-codes/{languageCode}` | Update localized description of a developer product |
| `GET` | `/legacy-game-internationalization/v1/developer-products/{developerProductId}/icons` | Get all icons for a developer product |
| `DELETE` | `/legacy-game-internationalization/v1/developer-products/{developerProductId}/icons/language-codes/{languageCode}` | Delete a localized icon from a developer product |
| `POST` | `/legacy-game-internationalization/v1/developer-products/{developerProductId}/icons/language-codes/{languageCode}` | Update a developer product's icon |
| `GET` | `/legacy-game-internationalization/v1/developer-products/{developerProductId}/name-description` | Get all names and descriptions of a developer product |
| `DELETE` | `/legacy-game-internationalization/v1/developer-products/{developerProductId}/name-description/language-codes/{languageCode}` | Delete localized name and description of a developer product |
| `PATCH` | `/legacy-game-internationalization/v1/developer-products/{developerProductId}/name-description/language-codes/{languageCode}` | Update localized name and description of a developer product |
| `PATCH` | `/legacy-game-internationalization/v1/developer-products/{developerProductId}/name/language-codes/{languageCode}` | Update localized name of a developer product |

### `PATCH` `/legacy-game-internationalization/v1/developer-products/{developerProductId}/description/language-codes/{languageCode}`

**Parameters:**

- `developerProductId` (path, integer (required)) - The developer product id
- `languageCode` (path, string (required)) - The language code of the description to update

**Request Body:** The request

**Responses:**

- `200` - OK
- `400` - 13: Request body can't be null 19: New name is null or whitespaces or new name/description is too l
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

### `GET` `/legacy-game-internationalization/v1/developer-products/{developerProductId}/icons`

**Parameters:**

- `developerProductId` (path, integer (required)) - The id of the developer product
- `width` (query, integer) - The width of the icon to request
- `height` (query, integer) - The height of the icon to request

**Responses:**

- `200` - OK
- `400` - 52: Image dimensions are invalid 70: Invalid developer product id
- `401` - 0: Authorization has been denied for this request.
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

### `DELETE` `/legacy-game-internationalization/v1/developer-products/{developerProductId}/icons/language-codes/{languageCode}`

**Parameters:**

- `developerProductId` (path, integer (required)) - The id of the developer product
- `languageCode` (path, string (required)) - The language code of the localized icon to delete

**Responses:**

- `200` - OK
- `400` - 22: Invalid language code 23: You can't delete translations for source language 53: Language is no
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

### `POST` `/legacy-game-internationalization/v1/developer-products/{developerProductId}/icons/language-codes/{languageCode}`

**Parameters:**

- `developerProductId` (path, integer (required)) - The id of the developer product
- `languageCode` (path, string (required)) - The language code of this icon to update

**Responses:**

- `200` - OK
- `400` - 22: Invalid language code 26: You can't update translations for source language 45: File uploaded 
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `429` - 24: Too many attempts.Please try again later.
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

### `GET` `/legacy-game-internationalization/v1/developer-products/{developerProductId}/name-description`

**Parameters:**

- `developerProductId` (path, integer (required)) - The developer product Id

**Responses:**

- `200` - OK
- `400` - 70: Invalid developer product id
- `401` - 0: Authorization has been denied for this request.
- `503` - 17: Feature is disabled

### `DELETE` `/legacy-game-internationalization/v1/developer-products/{developerProductId}/name-description/language-codes/{languageCode}`

**Parameters:**

- `developerProductId` (path, integer (required)) - The developer product id
- `languageCode` (path, string (required)) - The language code of the name and description to delete

**Responses:**

- `200` - OK
- `400` - 22: Invalid language code 23: You can't delete translations for source language 53: Language is no
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

### `PATCH` `/legacy-game-internationalization/v1/developer-products/{developerProductId}/name-description/language-codes/{languageCode}`

**Parameters:**

- `developerProductId` (path, integer (required)) - The developer product id
- `languageCode` (path, string (required)) - The language code of the name and description to Update

**Request Body:** The request

**Responses:**

- `200` - OK
- `400` - 13: Request body can't be null 19: New name is null or whitespaces or new name/description is too l
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

### `PATCH` `/legacy-game-internationalization/v1/developer-products/{developerProductId}/name/language-codes/{languageCode}`

**Parameters:**

- `developerProductId` (path, integer (required)) - The developer product id
- `languageCode` (path, string (required)) - The language code of the name to update

**Request Body:** The request

**Responses:**

- `200` - OK
- `400` - 13: Request body can't be null 19: New name is null or whitespaces or new name/description is too l
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 18: You do not have permission to manage this game
- `500` - 0: An unknown error occurred.
- `503` - 17: Feature is disabled

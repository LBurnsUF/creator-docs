---
title: V1 / Themes
type: cloud-api
tags: [Accounts]
---

# V1 / Themes

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/themes/{consumerType}/{consumerId}` | returns the theme type for a specific consumer. |
| `PATCH` | `/v1/themes/{consumerType}/{consumerId}` | Modify the theme type for consumer. |

### `GET` `/v1/themes/{consumerType}/{consumerId}`

**Parameters:**

- `consumerType` (path, integer (required)) - The consumer type
- `consumerId` (path, string (required)) - The consumer's theme configuration to get. If the consumerType is User always return the AuthenticatedUser's theme type.

**Responses:**

- `200` - OK
- `400` - 3: Invalid consumer type.
- `401` - 0: Authorization has been denied for this request.

### `PATCH` `/v1/themes/{consumerType}/{consumerId}`

**Parameters:**

- `consumerType` (path, integer (required)) - The consumer type
- `consumerId` (path, integer (required)) - The consumer's theme configuration to modify. If the consumerType is User always modify the AuthenticatedUser's theme type.

**Request Body:** An Roblox.AccountSettings.Api.ThemeConfigurationRequest.

**Responses:**

- `200` - OK
- `400` - 2: Invalid theme type.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

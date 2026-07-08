---
title: V1 / Account / Settings
type: cloud-api
tags: [Accounts]
---

# V1 / Account / Settings

Cloud API resource group with 3 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/account/settings/account-country` | Get a user's current account country setting. |
| `POST` | `/v1/account/settings/account-country` | Updates the user's account country. |
| `GET` | `/v1/account/settings/metadata` | Returns metadata used by the account settings page |

### `GET` `/v1/account/settings/account-country`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

### `POST` `/v1/account/settings/account-country`

**Responses:**

- `200` - OK
- `400` - 1: InvalidRequest
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: OperationNotPermitted
- `404` - 2: OperationNotPermitted
- `500` - 0: Unknown

### `GET` `/v1/account/settings/metadata`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

---
title: V1 / Users / Authenticated
type: cloud-api
tags: [Accounts]
---

# V1 / Users / Authenticated

Cloud API resource group with 4 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/users/authenticated` | Gets the minimal authenticated user. |
| `GET` | `/v1/users/authenticated/age-bracket` | Gets the age bracket of the authenticated user. |
| `GET` | `/v1/users/authenticated/country-code` | Gets the country code of the authenticated user. |
| `GET` | `/v1/users/authenticated/roles` | Gets the (public) roles of the authenticated user, such as `"Soothsayer"` and `"BetaTester"`. |

### `GET` `/v1/users/authenticated`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

### `GET` `/v1/users/authenticated/age-bracket`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

### `GET` `/v1/users/authenticated/country-code`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

### `GET` `/v1/users/authenticated/roles`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

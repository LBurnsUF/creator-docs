---
title: V1 / Email
type: cloud-api
tags: [Accounts]
---

# V1 / Email

Cloud API resource group with 3 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/email` | Gets the authenticated user's email address and verified status |
| `PATCH` | `/v1/email` | Updates the authenticated user's email address |
| `POST` | `/v1/email` | Updates the authenticated user's email address |

### `GET` `/v1/email`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

### `PATCH` `/v1/email`

**Responses:**

- `200` - OK
- `400` - 8: Password is incorrect. 9: Invalid email address.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: This feature is currently disabled. Please try again later. 3: There
- `409` - 4: This is already the current email.
- `429` - 6: Too many attempts to update email. Please try again later. 7: Too many attempts to send verifica
- `503` - 2: This feature is currently disabled. Please try again later.

### `POST` `/v1/email`

**Responses:**

- `200` - OK
- `400` - 8: Password is incorrect. 9: Invalid email address.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: This feature is currently disabled. Please try again later. 3: There
- `409` - 4: This is already the current email.
- `429` - 6: Too many attempts to update email. Please try again later. 7: Too many attempts to send verifica
- `503` - 2: This feature is currently disabled. Please try again later.

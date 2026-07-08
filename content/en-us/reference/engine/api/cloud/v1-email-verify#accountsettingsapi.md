---
title: V1 / Email / Verify#Accountsettingsapi
type: cloud-api
tags: [Accounts]
---

# V1 / Email / Verify#Accountsettingsapi

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/email/verify#AccountSettingsApi` | Send verify email to the authenticated user's email address |

### `POST` `/v1/email/verify#AccountSettingsApi`

**Request Body:** The request body.

**Responses:**

- `200` - OK
- `400` - 10: No email address is associated with the account.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 2: This feature is currently disabled. Please try again later. 11: You 
- `409` - 5: The email is already verified.
- `429` - 7: Too many attempts to send verification email. Please try again later.
- `503` - 2: This feature is currently disabled. Please try again later.

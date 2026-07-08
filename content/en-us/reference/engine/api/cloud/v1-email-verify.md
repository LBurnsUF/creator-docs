---
title: V1 / Email / Verify
type: cloud-api
tags: [Accounts]
---

# V1 / Email / Verify

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/email/verify` | Verify the user's email address from token |

### `POST` `/v1/email/verify`

**Request Body:** Roblox.AccountInformation.Api.Models.VerifyEmailRequest

**Responses:**

- `200` - OK
- `403` - 0: Token Validation Failed

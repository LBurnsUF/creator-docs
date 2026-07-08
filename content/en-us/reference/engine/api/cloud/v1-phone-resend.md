---
title: V1 / Phone / Resend
type: cloud-api
tags: [Accounts]
---

# V1 / Phone / Resend

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/phone/resend` | Resend Phone code |

### `POST` `/v1/phone/resend`

**Request Body:** Roblox.AccountInformation.Api.Models.PhoneRequest

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `429` - 6: Flooded
- `500` - 0: An unknown error occured.
- `503` - 1: This feature is currently disabled. Please try again later.

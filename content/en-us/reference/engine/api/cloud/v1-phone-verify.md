---
title: V1 / Phone / Verify
type: cloud-api
tags: [Accounts]
---

# V1 / Phone / Verify

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/phone/verify` | Verify Phone |

### `POST` `/v1/phone/verify`

**Request Body:** Roblox.AccountInformation.Api.Models.VerifyPhoneRequest

**Responses:**

- `200` - OK
- `400` - 2: Invalid Phone Number 3: Phone Number Already Associated 7: Invalid Code
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `429` - 6: Flooded
- `500` - 0: An unknown error occured.
- `503` - 1: This feature is currently disabled. Please try again later.

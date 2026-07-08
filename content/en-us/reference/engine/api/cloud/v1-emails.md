---
title: V1 / Emails
type: cloud-api
tags: [Accounts]
---

# V1 / Emails

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/emails` | Gets the authenticated user's verified email and pending (unverified) email if one exists |

### `GET` `/v1/emails`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

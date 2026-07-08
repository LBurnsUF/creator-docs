---
title: V1 / Messages / Unarchive
type: cloud-api
tags: [Accounts]
---

# V1 / Messages / Unarchive

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/messages/unarchive` | Unarchives a batch of messages. |

### `POST` `/v1/messages/unarchive`

**Responses:**

- `200` - OK
- `400` - 5: Too many ids in a batch request.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

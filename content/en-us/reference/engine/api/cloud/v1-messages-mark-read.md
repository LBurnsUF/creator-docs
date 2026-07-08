---
title: V1 / Messages / Mark Read
type: cloud-api
tags: [Accounts]
---

# V1 / Messages / Mark Read

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/messages/mark-read` | Marks a batch of messages as read. |

### `POST` `/v1/messages/mark-read`

**Responses:**

- `200` - OK
- `400` - 5: Too many ids in a batch request.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

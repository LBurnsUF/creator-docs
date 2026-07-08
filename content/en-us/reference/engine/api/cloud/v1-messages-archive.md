---
title: V1 / Messages / Archive
type: cloud-api
tags: [Accounts]
---

# V1 / Messages / Archive

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/messages/archive` | Archives a batch of messages. |

### `POST` `/v1/messages/archive`

**Responses:**

- `200` - OK
- `400` - 5: Too many ids in a batch request.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

---
title: V1 / Groups / Policies
type: cloud-api
tags: [Groups]
---

# V1 / Groups / Policies

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/groups/policies` | Gets group policy info used for compliance. |

### `POST` `/v1/groups/policies`

**Responses:**

- `200` - OK
- `400` - 1: Too many ids in request. 2: Ids could not be parsed from request.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

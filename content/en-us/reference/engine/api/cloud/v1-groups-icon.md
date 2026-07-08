---
title: V1 / Groups / Icon
type: cloud-api
tags: [Groups, Thumbnails]
---

# V1 / Groups / Icon

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `PATCH` | `/v1/groups/icon` | Updates the group icon. |

### `PATCH` `/v1/groups/icon`

**Parameters:**

- `groupId` (query, integer (required)) - The group Id.

**Responses:**

- `200` - OK
- `400` - 1: Group is invalid or does not exist. 16: The group icon is missing from the request. 17: Too man
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 23: Insufficient permissions to complete the request.
- `413` - 0: Unknown error.

---
title: V1 / User / Get Tags
type: cloud-api
tags: [Users]
---

# V1 / User / Get Tags

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/user/get-tags` | Gets the tags for multiple users |

### `POST` `/v1/user/get-tags`

**Responses:**

- `200` - OK
- `400` - 4: Invalid parameters. 8: Too many user Tags are requested.
- `401` - 0: Authorization has been denied for this request.
- `429` - 10: The flood limit has been exceeded.

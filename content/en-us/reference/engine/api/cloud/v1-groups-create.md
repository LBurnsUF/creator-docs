---
title: V1 / Groups / Create
type: cloud-api
tags: [Groups]
---

# V1 / Groups / Create

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/groups/create` | Creates a new group. |

### `POST` `/v1/groups/create`

This endpoint will charge Robux for the group purchase.
Accepts "icon" and "coverPhoto" in Files object. Defaults to first file if "icon" is not present.
Http status code 413 is thrown when the group icon file size is too large.

**Responses:**

- `200` - OK
- `400` - 13: The name is invalid. 15: The group icon is invalid. 16: The group icon is missing from the req
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 10: User must have builders club membership. 11: User is in maximum num
- `409` - 37: The name was in use too recently.
- `413` - 0: Unknown error.
- `429` - 17: Too many requests.
- `503` - 21: Group creation is currently disabled.

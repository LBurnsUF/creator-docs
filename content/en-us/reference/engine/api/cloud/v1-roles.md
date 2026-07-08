---
title: V1 / Roles
type: cloud-api
tags: [Groups]
---

# V1 / Roles

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/roles` | Gets the Roles by their ids. |

### `GET` `/v1/roles`

**Parameters:**

- `ids` (query, array (required)) - A list of role ids

**Responses:**

- `200` - OK
- `400` - 1: Ids could not be parsed from request. 2: Too many ids in request.

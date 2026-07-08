---
title: V1 / Catalog / Items
type: cloud-api
tags: [Assets, Avatars]
---

# V1 / Catalog / Items

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/catalog/items/details` | Returns details for one or more catalog items. |

### `POST` `/v1/catalog/items/details`

There is an item count limit per request. Exceeding this returns 400 Bad Request.

**Request Body:** Roblox.Catalog.Api.MultigetItemDetailsRequestModel.

**Responses:**

- `200` - OK
- `400` - 2: Invalid count
- `403` - 0: Token Validation Failed 7: User is unauthorized.
- `429` - 8: The flood limit has been exceeded.

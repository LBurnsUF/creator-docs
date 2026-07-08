---
title: V1 / Games / Games Product Info
type: cloud-api
tags: [Universes]
---

# V1 / Games / Games Product Info

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/games/games-product-info` | Gets a list of games' product info, used to purchase a game |

### `GET` `/v1/games/games-product-info`

**Parameters:**

- `universeIds` (query, array (required)) - A list of universe Ids. Cannot exceed a maximum of 100 IDs.

**Responses:**

- `200` - OK
- `400` - 8: The universe IDs specified are invalid. 9: Too many universe IDs were requested.

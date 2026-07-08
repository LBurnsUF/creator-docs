---
title: V1 / Games / Multiget Place Details
type: cloud-api
tags: [Places, Universes]
---

# V1 / Games / Multiget Place Details

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/games/multiget-place-details` | Get place details |

### `GET` `/v1/games/multiget-place-details`

**Parameters:**

- `placeIds` (query, array (required)) - List of placeId to uniquely Identify a place

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

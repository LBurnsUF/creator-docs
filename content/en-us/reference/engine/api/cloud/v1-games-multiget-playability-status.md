---
title: V1 / Games / Multiget Playability Status
type: cloud-api
tags: [Accounts, Universes]
---

# V1 / Games / Multiget Playability Status

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/games/multiget-playability-status` | Gets a list of universe playability statuses for the authenticated user |

### `GET` `/v1/games/multiget-playability-status`

**Parameters:**

- `universeIds` (query, array (required)) - A list of universe Ids. Cannot exceed a maximum of 50 IDs.

**Responses:**

- `200` - OK
- `400` - 8: The universe IDs specified are invalid. 9: Too many universe IDs were requested.

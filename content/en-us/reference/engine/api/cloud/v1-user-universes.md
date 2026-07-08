---
title: V1 / User / Universes
type: cloud-api
tags: [Universes]
---

# V1 / User / Universes

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/user/universes` | Gets a list of universes for the authenticated user. |

### `GET` `/v1/user/universes`

**Parameters:**

- `isArchived` (query, boolean) - Whether or not to return archived games.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.
- `sortOrder` (query, string) - Sorted by universeId

**Responses:**

- `200` - OK
- `400` - cursor is not valid.
- `401` - 0: Authorization has been denied for this request.

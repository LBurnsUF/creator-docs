---
title: Legacy Develop / V1 / Places
type: cloud-api
tags: [Places, Team Create, Universes]
---

# Legacy Develop / V1 / Places

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/legacy-develop/v1/places/{placeId}/teamcreate/active_session/members` | List of users in the active Team Create session |

### `GET` `/legacy-develop/v1/places/{placeId}/teamcreate/active_session/members`

**Parameters:**

- `placeId` (path, integer (required)) - The place Id.
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.

**Responses:**

- `200` - OK
- `400` - 1: The universe is invalid. 5: The place is invalid.
- `401` - 0: Authorization has been denied for this request.
- `403` - 2: Not authorized to perform this action. 4: TeamCreate on universe is disabled.
- `404` - 0: An unknown error occurred.
- `500` - 6: Multiple active sessions in a Team Create place.

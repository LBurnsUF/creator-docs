---
title: V1 / Users / Search
type: cloud-api
tags: [Users]
---

# V1 / Users / Search

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/users/search` | Searches for users by keyword. |

### `GET` `/v1/users/search`

**Parameters:**

- `keyword` (query, string (required)) - The search keyword.
- `sessionId` (query, string) - 
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.

**Responses:**

- `200` - OK
- `400` - 5: The keyword was filtered. 6: The keyword is too short.
- `429` - 4: Too many requests.

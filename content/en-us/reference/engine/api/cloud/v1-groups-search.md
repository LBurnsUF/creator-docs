---
title: V1 / Groups / Search
type: cloud-api
tags: [Groups, Metadata]
---

# V1 / Groups / Search

Cloud API resource group with 3 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/groups/search` | Search for groups by keyword. |
| `GET` | `/v1/groups/search/lookup` | Looks up groups by a name. Prioritizes an exact match as the first result. |
| `GET` | `/v1/groups/search/metadata` | Get suggested groups and other miscellaneous information needed for the group/join page like flags |

### `GET` `/v1/groups/search`

**Parameters:**

- `keyword` (query, string (required)) - The keyword or phrase to use as the search parameter.
- `prioritizeExactMatch` (query, boolean) - Whether or not to prioritize the exact match for the keyword (optional, defaults to false).
- `limit` (query, integer) - The number of results per request.
- `cursor` (query, string) - The paging cursor for the previous or next page.

**Responses:**

- `200` - OK
- `400` - 2: Search term not appropriate for Roblox. 3: Search term was left empty. 4: Search terms can be 2

### `GET` `/v1/groups/search/lookup`

Should only be used for direct lookups where a user is inputting a group name, shouldn't be used for search pages.

**Parameters:**

- `groupName` (query, string (required)) - The group name.

**Responses:**

- `200` - OK
- `400` - 1: Name is missing or has invalid characters.

### `GET` `/v1/groups/search/metadata`

Although there is no reason for this to require an authenticated user right now, in the future,
we will use coco to return different suggested groups based upon that user's request context

**Responses:**

- `200` - OK
- `404` - 5: No Localized Version of group search category exists

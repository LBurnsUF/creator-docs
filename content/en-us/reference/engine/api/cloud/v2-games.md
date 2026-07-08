---
title: V2 / Games
type: cloud-api
tags: [Thumbnails, Universes]
---

# V2 / Games

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/games/{universeId}/media` | Get the game media data |

### `GET` `/v2/games/{universeId}/media`

**Parameters:**

- `universeId` (path, integer (required)) - The id of the universe we get media data from.
- `fetchAllExperienceRelatedMedia` (query, boolean) - to tell if the API query is to fetch all related media for this experience

**Responses:**

- `200` - OK
- `400` - 3: The universe's root place is invalid.
- `404` - 2: The requested universe does not exist.

---
title: V2 / Teamtest
type: cloud-api
tags: [Places, Team Create]
---

# V2 / Teamtest

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `DELETE` | `/v2/teamtest/{placeId}` | Close a game instance that is being used for team testing |

### `DELETE` `/v2/teamtest/{placeId}`

**Parameters:**

- `placeId` (path, integer (required)) - The Id of the place we are setting the metadata for.
- `gameId` (query, string (required)) - the Guid of the game instance System.Guid

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

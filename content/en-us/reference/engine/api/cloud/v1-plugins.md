---
title: V1 / Plugins
type: cloud-api
tags: [Assets]
---

# V1 / Plugins

Cloud API resource group with 3 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/plugins` | Gets plugin details by ids. |
| `PATCH` | `/v1/plugins/{pluginId}` | Updates a plugin. |
| `POST` | `/v1/plugins/{pluginId}/icon` | Overwrites a plugin icon with a new one. |

### `GET` `/v1/plugins`

**Parameters:**

- `pluginIds` (query, array (required)) - The plugin ids.

**Responses:**

- `200` - OK
- `400` - 1: Too many ids. 2: The format of the ids are invalid.

### `PATCH` `/v1/plugins/{pluginId}`

**Parameters:**

- `pluginId` (path, integer (required)) - The id of the plugin.

**Request Body:** The Roblox.Develop.Api.UpdatePluginRequest.

**Responses:**

- `200` - OK
- `400` - 5: Description too long. 6: Text moderated. 7: Invalid name. 8: The request body is missing.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 4: Insufficient permissions.
- `404` - 3: The id is invalid.

### `POST` `/v1/plugins/{pluginId}/icon`

**Parameters:**

- `pluginId` (path, integer (required)) - The plugin Id.

**Responses:**

- `200` - OK
- `400` - 2: File not present in request.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 5: You do not have permission to manage this item.
- `404` - 4: Target item is invalid or does not exist.
- `429` - 3: You're uploading too much, please wait and try again later.

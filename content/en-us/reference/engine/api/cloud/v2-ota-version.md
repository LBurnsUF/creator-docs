---
title: V2 / Ota Version
type: cloud-api
tags: [Metadata]
---

# V2 / Ota Version

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/ota-version/{binaryType}` | Get OTA information for a specific binary type with a given version on some channel. Returns empty  |

### `GET` `/v2/ota-version/{binaryType}`

**Parameters:**

- `binaryType` (path, string (required)) - Binary type of the application to get info for
- `channel` (query, string) - Channel name. If not provided, production is assumed.
- `version` (query, string) - Application version
- `tag` (query, string) - Tag to filter results by. Only applicable to non-studio application types.
- `name` (query, string) - Name to filter results by. Only applicable to non-studio application types.

**Responses:**

- `200` - OK
- `400` - 2: Invalid binaryType. 4: Invalid app version. 6: Missing or invalid channel. 7: Unsupported bina
- `401` - 5: Not authorized to perform this action.

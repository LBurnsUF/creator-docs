---
title: V2 / Client Version
type: cloud-api
tags: [Metadata]
---

# V2 / Client Version

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/client-version/{binaryType}` | Get client version information for specific binary type |
| `GET` | `/v2/client-version/{binaryType}/channel/{channelName}` | Get client version information for specific binary type |

### `GET` `/v2/client-version/{binaryType}`

**Parameters:**

- `binaryType` (path, string (required)) - Platform(WindowsPlayer, WindowsStudio, MacPlayer or MacStudio) for which we want the latest version

**Responses:**

- `200` - OK

### `GET` `/v2/client-version/{binaryType}/channel/{channelName}`

**Parameters:**

- `binaryType` (path, string (required)) - Platform(WindowsPlayer, WindowsStudio, MacPlayer or MacStudio) for which we want the latest version
- `channelName` (path, string (required)) - Channel Name

**Responses:**

- `200` - OK
- `401` - 5: Not authorized to perform this action.

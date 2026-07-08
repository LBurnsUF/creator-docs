---
title: V1 / Client Version
type: cloud-api
tags: [Metadata]
---

# V1 / Client Version

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/client-version/{binaryType}` | Get client version information for specific binary type |

### `GET` `/v1/client-version/{binaryType}`

**Parameters:**

- `binaryType` (path, string (required)) - Platform(WindowsPlayer, WindowsStudio, MacPlayer or MacStudio) for which we want the latest version

**Responses:**

- `200` - OK

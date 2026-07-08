---
title: V1 / Mobile Client Version
type: cloud-api
tags: [Metadata]
---

# V1 / Mobile Client Version

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/mobile-client-version` | Get mobile client version information based on app version parameter |

### `GET` `/v1/mobile-client-version`

**Parameters:**

- `appVersion` (query, string (required)) - AppiOSV2.13, AppVersioniOS2.0.1, etc

**Responses:**

- `200` - OK
- `400` - 2: Invalid binaryType.

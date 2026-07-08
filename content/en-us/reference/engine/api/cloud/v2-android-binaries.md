---
title: V2 / Android Binaries
type: cloud-api
tags: [Metadata]
---

# V2 / Android Binaries

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/android-binaries/{version}/channels/{channelName}` | Retrieve the Android binary information for a given version and channel name. |

### `GET` `/v2/android-binaries/{version}/channels/{channelName}`

**Parameters:**

- `version` (path, string (required)) - The version string of the application. i.e. 2.660.392
- `channelName` (path, string (required)) - The name of the channel. E.g. ZFlag, ZIntegration

**Responses:**

- `200` - OK

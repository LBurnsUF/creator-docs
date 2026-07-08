---
title: V2 / Marassethash
type: cloud-api
tags: [Assets]
---

# V2 / Marassethash

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/marAssetHash/{marAssetHash}/marCheckSum/{marCheckSum}` |  |

### `GET` `/v2/marAssetHash/{marAssetHash}/marCheckSum/{marCheckSum}`

**Parameters:**

- `marAssetHash` (path, string (required)) - 
- `marCheckSum` (path, string (required)) - 
- `Accept-Encoding` (header, string (required)) - 
- `Roblox-Place-Id` (header, integer (required)) - 
- `AssetType` (header, string (required)) - 
- `Accept` (header, string (required)) - 
- `AssetFormat` (header, string (required)) - 
- `Roblox-AssetFormat` (header, string (required)) - 
- `skipSigningScripts` (query, boolean) - 
- `clientInsert` (query, integer) - 
- `scriptinsert` (query, integer) - 
- `modulePlaceId` (query, integer) - 
- `serverplaceid` (query, integer) - 
- `expectedAssetType` (query, string) - 

**Responses:**

- `200` - OK

---
title: V1 / Marassethash
type: cloud-api
tags: [Assets]
---

# V1 / Marassethash

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/marAssetHash/{marAssetHash}/marCheckSum/{marCheckSum}` | Retrieves an asset by its mar (moderation agnostic) hash and mar (moderation agnostic) checksum. |

### `GET` `/v1/marAssetHash/{marAssetHash}/marCheckSum/{marCheckSum}`

**Parameters:**

- `marAssetHash` (path, string (required)) - The mar (moderation agnostic) hash of the asset to retrieve.
- `marCheckSum` (path, string (required)) - The mar (moderation agnostic) checksum of the asset to retrieve.
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
- `400` - 2: invalid server request 3: Encoding cannot be empty
- `404` - 5: Asset hash cannot be empty

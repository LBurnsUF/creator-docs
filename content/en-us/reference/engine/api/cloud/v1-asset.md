---
title: V1 / Asset
type: cloud-api
tags: [Assets]
---

# V1 / Asset

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/asset` |  |

### `GET` `/v1/asset`

**Parameters:**

- `Accept-Encoding` (header, string (required)) - 
- `Roblox-Place-Id` (header, integer (required)) - 
- `AssetType` (header, string (required)) - 
- `Accept` (header, string (required)) - 
- `AssetFormat` (header, string (required)) - 
- `Roblox-AssetFormat` (header, string (required)) - 
- `id` (query, integer) - 
- `userAssetId` (query, integer) - 
- `assetVersionId` (query, integer) - 
- `version` (query, integer) - 
- `universeId` (query, integer) - 
- `clientInsert` (query, integer) - 
- `scriptinsert` (query, integer) - 
- `modulePlaceId` (query, integer) - 
- `serverplaceid` (query, string) - 
- `assetName` (query, string) - 
- `hash` (query, string) - 
- `marAssetHash` (query, string) - 
- `marCheckSum` (query, string) - 
- `expectedAssetType` (query, string) - 
- `skipSigningScripts` (query, boolean) - 
- `permissionContext` (query, string) - 
- `doNotFallbackToBaselineRepresentation` (query, boolean) - 
- `contentRepresentationPriorityList` (query, string) - 
- `assetResolutionMode` (query, string) - 
- `accessContext` (query, string) - 
- `usageContext` (query, integer) - 

**Responses:**

- `200` - OK

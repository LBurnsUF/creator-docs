---
title: V2 / Assetid
type: cloud-api
tags: [Assets]
---

# V2 / Assetid

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/assetId/{assetId}` |  |
| `GET` | `/v2/assetId/{assetId}/version/{versionNumber}` |  |

### `GET` `/v2/assetId/{assetId}`

**Parameters:**

- `assetId` (path, integer (required)) - 
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
- `doNotFallbackToBaselineRepresentation` (query, boolean) - 
- `contentRepresentationPriorityList` (query, string) - 
- `accessContext` (query, string) - 
- `usageContext` (query, integer) - 

**Responses:**

- `200` - OK

### `GET` `/v2/assetId/{assetId}/version/{versionNumber}`

**Parameters:**

- `assetId` (path, integer (required)) - 
- `versionNumber` (path, integer (required)) - 
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
- `doNotFallbackToBaselineRepresentation` (query, boolean) - 
- `contentRepresentationPriorityList` (query, string) - 
- `accessContext` (query, string) - 
- `usageContext` (query, integer) - 

**Responses:**

- `200` - OK

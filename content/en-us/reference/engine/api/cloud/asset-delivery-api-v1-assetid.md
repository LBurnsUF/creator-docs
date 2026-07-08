---
title: Asset Delivery Api / V1 / Assetid
type: cloud-api
tags: [Assets]
---

# Asset Delivery Api / V1 / Assetid

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/asset-delivery-api/v1/assetId/{assetId}` | Retrieves an asset by its ID with OpenCloud auth. |
| `GET` | `/asset-delivery-api/v1/assetId/{assetId}/version/{versionNumber}` | Retrieves an asset by its ID and version number with OpenCloud auth. |

### `GET` `/asset-delivery-api/v1/assetId/{assetId}`

Returns an object containing a `location` property which is a temporary CDN URL for the asset content. All asset types are supported.
You should request that URL with the `Accept-Encoding: gzip` header and decompress the result if the response is gzipped. If you are using cURL, the `--compressed` flag will automate these steps for you.
This endpoint is expected to be called with API key authentication through `apis.roblox.com/asset-delivery-api/v1/assetId/{assetId}`.
While you are able to make requests to this endpoint with Cookie authentication via `assetdelivery.roblox.com/v1/openCloud/assetId/{assetId}`, we highly discourage use this way.
Expect unannounced removal of this second route in the future.

**Parameters:**

- `assetId` (path, integer (required)) - The ID of the asset to retrieve.
- `Accept-Encoding` (header, string) - The Accept-Encoding header value specifying compression formats (e.g., "gzip, deflate"). Defaults to "gzip, deflate" if not provided.
- `Roblox-Place-Id` (header, integer) - The Roblox-Place-Id header value identifying the place making the request.
- `AssetType` (header, string) - The AssetType header value specifying the expected asset type.
- `Accept` (header, string) - The Accept header value specifying the preferred response content type.
- `AssetFormat` (header, string) - The AssetFormat header value specifying the desired asset format. Overridden by robloxAssetFormat if both are provided.
- `Roblox-AssetFormat` (header, string) - The Roblox-AssetFormat header value specifying the preferred Roblox-specific asset format. Takes precedence over assetFormat.
- `skipSigningScripts` (query, boolean) - Whether to skip script signing for the returned asset. Used for script assets that don't require signing.
- `clientInsert` (query, integer) - Set to 1 to indicate this is a client insert request.
- `scriptinsert` (query, integer) - Set to 1 to indicate this is a script insert request.
- `modulePlaceId` (query, integer) - The place ID of the module making the request.
- `serverplaceid` (query, integer) - The server place ID making the request.
- `expectedAssetType` (query, string) - The expected asset type as a fallback when assetType header is not provided.
- `doNotFallbackToBaselineRepresentation` (query, boolean) - Whether to prevent fallback to baseline representation when specific content representations are not available.
- `contentRepresentationPriorityList` (query, string) - Base64URL-encoded JSON string specifying the priority list of desired content representations (format, version, fidelity).
- `accessContext` (query, string) - 
- `usageContext` (query, integer) - 

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.

### `GET` `/asset-delivery-api/v1/assetId/{assetId}/version/{versionNumber}`

Refer to the assetId endpoint for details on usage.
This endpoint is expected to be called with API key authentication through `apis.roblox.com/asset-delivery-api/v1/assetId/{assetId}/version/{versionNumber}`.
While you are able to make requests to this endpoint with Cookie authentication via `assetdelivery.roblox.com/v1/openCloud/assetId/{assetId}/version/{versionNumber}`, we highly discourage use this way.
Expect unannounced removal of this second route in the future.

**Parameters:**

- `assetId` (path, integer (required)) - The ID of the asset to retrieve.
- `versionNumber` (path, integer (required)) - The version number of the asset to retrieve.
- `Accept-Encoding` (header, string) - 
- `Roblox-Place-Id` (header, integer) - 
- `AssetType` (header, string) - 
- `Accept` (header, string) - 
- `AssetFormat` (header, string) - 
- `Roblox-AssetFormat` (header, string) - 
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
- `401` - 0: Authorization has been denied for this request.

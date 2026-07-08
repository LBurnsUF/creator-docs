---
title: Assets / V1 / Assets
type: cloud-api
tags: [Assets]
---

# Assets / V1 / Assets

Cloud API resource group with 8 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/assets/v1/assets` | Creates an asset with provided content and metadata. [BETA] |
| `GET` | `/assets/v1/assets/{assetId}` | Retrieve specific asset metadata. Include the `readMask` parameter for additional asset metadata. [BETA] |
| `PATCH` | `/assets/v1/assets/{assetId}` | Updates an asset with provided content and metadata. [BETA] |
| `GET` | `/assets/v1/assets/{assetId}/versions` | List Asset Versions of an Asset [BETA] |
| `GET` | `/assets/v1/assets/{assetId}/versions/{versionNumber}` | Get Asset Version [BETA] |
| `POST` | `/assets/v1/assets/{assetId}/versions:rollback` | Rollback an asset to a previous version. [BETA] |
| `POST` | `/assets/v1/assets/{assetId}:archive` | Archives the asset. [BETA] |
| `POST` | `/assets/v1/assets/{assetId}:restore` | Restores an archived asset. [BETA] |

### `POST` `/assets/v1/assets`

**Operation:** `Assets_CreateAsset`

**Stability:** BETA

Creates an asset with provided content and metadata.

You can't add [SocialLink](#SocialLink) objects when you create an asset. Instead, use [Update Asset](#PATCH-v1-assets-_assetId_).

Provide the [Asset](#Asset), binary asset file path, and [content type](/cloud/guides/usage-assets.md#supported-asset-types-and-limits) in the form data.

**Responses:**

- `200` - Returns the Operation ID for checking the creation status.
- `400` - Invalid argument. Failed to parse the request or the file.
- `401` - The API key is not valid for this operation / You don't have the authorization.
- `500` - Server internal error / Unknown error.

### `GET` `/assets/v1/assets/{assetId}`

**Operation:** `Assets_GetAsset`

**Stability:** BETA

Retrieve specific asset metadata.

**Parameters:**

- `assetId` (path, string (required)) - The unique identifier of the asset.
- `readMask` (query, string) - Asset metadata fields to retrieve, including the description, display name, icon, social links, and previews. Examples: `description%2CdisplayName`, `

**Responses:**

- `200` - Asset resource retrieved successfully.
- `400` - Malformed request, likely due to an invalid read mask.
- `401` - The API key is not valid for this operation / You don't have the authorization.
- `403` - Doesn't have the required permission.
- `404` - Asset doesn't exist.
- `500` - Server internal error / Unknown error.

### `PATCH` `/assets/v1/assets/{assetId}`

**Operation:** `Assets_UpdateAsset`

**Stability:** BETA

Updates an asset with provided content and metadata, including the description, display name, icon, social links, and previews. Currently can only update the content body for **Models**. Icons and Previews must be **Image** assets. Icons must have square dimensions.

Provide the [Asset](#Asset), binary asset file path, and [content type](/cloud/guides/usage-assets.md#supported-asset-types-and-limits) in the form data.

**Parameters:**

- `assetId` (path, string (required)) - The unique identifier of the asset.
- `updateMask` (query, string) - Asset metadata fields to update, including the description, display name, icon, and previews. Examples: `description%2CdisplayName`, `previews%2Ctwitc

**Responses:**

- `200` - Returns the Operation ID for checking the update status / Returns the updated metadata fields.
- `400` - Invalid argument. Failed to parse the request or the file.
- `401` - The API key is not valid for this operation / You don't have the authorization.
- `500` - Server internal error / Unknown error.

### `GET` `/assets/v1/assets/{assetId}/versions`

**Operation:** `listAssetVersions`

**Stability:** BETA

List all versions of a specific asset, with optional pagination.

**Parameters:**

- `assetId` (path, string (required)) - The unique identifier of the asset.
- `maxPageSize` (query, integer) - Specifies the number of asset versions to include in the response. Valid values range from 1 to 50 (inclusive). Defaults to 8 when not provided.
- `pageToken` (query, string) - A token for pagination. The value is obtained from a previous request and allows for retrieving the next page of asset versions.

**Responses:**

- `200` - Asset versions listed successfully.
- `400` - Bad request - invalid parameters.
- `403` - Forbidden - API key without Read scope or user doesn't have access.
- `404` - Asset not found.

### `GET` `/assets/v1/assets/{assetId}/versions/{versionNumber}`

**Operation:** `Assets_GetAssetVersion`

**Stability:** BETA

Retrieve a specific asset version by the asset ID and the version number.

**Parameters:**

- `assetId` (path, string (required)) - The unique identifier of the asset.
- `versionNumber` (path, string (required)) - The version number.

**Responses:**

- `200` - Asset version retrieved successfully.
- `403` - Forbidden - API key without Read scope or user doesn't have access.
- `404` - Asset or Asset Version not found.

### `POST` `/assets/v1/assets/{assetId}/versions:rollback`

**Operation:** `Assets_RollbackAssetVersion`

**Stability:** BETA

Rollback an asset to a specific previous version.

 Provide the asset version path in the form data.

**Parameters:**

- `assetId` (path, string (required)) - The unique identifier of the asset.

**Responses:**

- `200` - Asset rolled back successfully.
- `400` - Bad request - invalid request body.
- `403` - Forbidden - API key without Write scope or user doesn't have access.
- `404` - Asset or Asset Version not found.

### `POST` `/assets/v1/assets/{assetId}:archive`

**Operation:** `Assets_ArchiveAsset`

**Stability:** BETA

Archives the asset. Archived assets disappear from the website and are no longer usable or visible in Roblox experiences, but you can [restore](#POST-v1-assets-{assetId}:restore) them.

**Parameters:**

- `assetId` (path, string (required)) - The unique identifier of the asset.

**Responses:**

- `200` - Asset archived succesfully successfully.
- `400` - Bad request - invalid request.
- `403` - Forbidden - API key without Write scope or user doesn't have access.
- `404` - Asset not found.

### `POST` `/assets/v1/assets/{assetId}:restore`

**Operation:** `Assets_RestoreAsset`

**Stability:** BETA

Restores an archived asset.

**Parameters:**

- `assetId` (path, string (required)) - The unique identifier of the asset.

**Responses:**

- `200` - Asset restored successfully.
- `400` - Bad request - invalid request.
- `403` - Forbidden - API key without Write scope or user doesn't have access.
- `404` - Asset not found.

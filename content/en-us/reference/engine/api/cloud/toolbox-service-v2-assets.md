---
title: Toolbox Service / V2 / Assets
type: cloud-api
tags: [Assets, Creator Store]
---

# Toolbox Service / V2 / Assets

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/toolbox-service/v2/assets/{id}` | Get Creator Store Asset Details [BETA] |

### `GET` `/toolbox-service/v2/assets/{id}`

**Operation:** `Toolbox_GetAssetDetails`

**Stability:** BETA

Get details for a single Creator Store asset.

**Parameters:**

- `id` (path, integer (required)) - The asset ID to retrieve details for.

**Responses:**

- `200` - Success
- `403` - Forbidden
- `404` - Not Found
- `429` - Too Many Requests

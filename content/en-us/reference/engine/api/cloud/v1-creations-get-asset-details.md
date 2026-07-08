---
title: V1 / Creations / Get Asset Details
type: cloud-api
tags: [Assets]
---

# V1 / Creations / Get Asset Details

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/creations/get-asset-details` | Gets the asset status and other configuration details for the given assetIds list. |

### `POST` `/v1/creations/get-asset-details`

**Responses:**

- `200` - OK
- `400` - 1: Missing AssetIds parameters 2: Invalid asset Ids
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed
- `414` - 3: Too many asset Ids
- `429` - 9: Flood Limit Exceeded
- `503` - 6: Service Unavailable

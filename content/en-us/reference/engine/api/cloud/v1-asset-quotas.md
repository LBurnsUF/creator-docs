---
title: V1 / Asset Quotas
type: cloud-api
tags: [Assets]
---

# V1 / Asset Quotas

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/asset-quotas` | List asset quotas of the given resource type and asset type. |

### `GET` `/v1/asset-quotas`

**Parameters:**

- `resourceType` (query, string (required)) - Resource type of the asset quota
- `assetType` (query, string (required)) - Asset type of the asset quota
- `useDummyData` (query, boolean) - Use dummy data for testing. This is for internal use only

**Responses:**

- `200` - OK
- `400` - 7: The asset type is not appropriate for this request. 8: The resource type is not appropriate for 
- `401` - 0: Authorization has been denied for this request.
- `500` - 0: Reserved for base level errors. Do not use in your endpoint directly, do not document.

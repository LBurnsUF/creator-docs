---
title: Cloud / V2 / Creator Store Products
type: cloud-api
tags: [Creator Store]
---

# Cloud / V2 / Creator Store Products

Cloud API resource group with 3 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/cloud/v2/creator-store-products` | Create Creator Store Product [BETA] |
| `GET` | `/cloud/v2/creator-store-products/{creator_store_product_id}` | Get Creator Store Product [BETA] |
| `PATCH` | `/cloud/v2/creator-store-products/{creator_store_product_id}` | Update Creator Store Product [BETA] |

### `POST` `/cloud/v2/creator-store-products`

**Operation:** `Cloud_CreateCreatorStoreProduct`

**Stability:** BETA

Add a Creator Store product. Only use this method if your product has never
been distributed on the Creator Store; otherwise, use the `PATCH` method to
update the product.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/creator-store-products/{creator_store_product_id}`

**Operation:** `Cloud_GetCreatorStoreProduct`

**Stability:** BETA

Get a Creator Store product.

**Parameters:**

- `creator_store_product_id` (path, string (required)) - The creator-store-product ID.

**Responses:**

- `200` - OK

### `PATCH` `/cloud/v2/creator-store-products/{creator_store_product_id}`

**Operation:** `Cloud_UpdateCreatorStoreProduct`

**Stability:** BETA

Update a Creator Store product.

**Parameters:**

- `creator_store_product_id` (path, string (required)) - The creator-store-product ID.
- `updateMask` (query, string) - The list of fields to update.
- `allowMissing` (query, boolean) - If set to true, and the creator store product is not found, a creator store product is created. In this situation, `update_mask` is ignored.

**Responses:**

- `200` - OK

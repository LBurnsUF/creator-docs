---
title: V1 / Collections / Items
type: cloud-api
tags: [Inventories]
---

# V1 / Collections / Items

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `DELETE` | `/v1/collections/items/{itemType}/{itemTargetId}` | Removes an item to the appropriate collection |
| `POST` | `/v1/collections/items/{itemType}/{itemTargetId}` | Adds an item to the appropriate collection |

### `DELETE` `/v1/collections/items/{itemType}/{itemTargetId}`

**Parameters:**

- `itemType` (path, integer (required)) - Type of the item (i.e. Asset, Bundle)
- `itemTargetId` (path, integer (required)) - ID of the item

**Responses:**

- `200` - OK
- `400` - 1: The item type does not exist. 2: The asset does not exist. 3: The bundle does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 8: The item is not in the collection.

### `POST` `/v1/collections/items/{itemType}/{itemTargetId}`

**Parameters:**

- `itemType` (path, integer (required)) - Type of the item (i.e. Asset, Bundle)
- `itemTargetId` (path, integer (required)) - ID of the item

**Responses:**

- `200` - OK
- `400` - 1: The item type does not exist. 2: The asset does not exist. 3: The bundle does not exist.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 4: You don't own the specified item. 5: Assets of this type are not all

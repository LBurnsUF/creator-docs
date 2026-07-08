---
title: V1 / Packages
type: cloud-api
tags: [Inventories]
---

# V1 / Packages

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/packages/{packageId}/assets` | Given a package ID, returns the list of asset IDs for that package **DEPRECATED** |

### `GET` `/v1/packages/{packageId}/assets`

> **Deprecated**

Packages have been migrated to bundles. Use catalog.roblox.com/v1/bundles/{bundleId}/details

**Parameters:**

- `packageID` (path, integer (required)) - The asset ID of the package

**Responses:**

- `200` - OK

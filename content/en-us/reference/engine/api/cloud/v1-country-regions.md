---
title: V1 / Country Regions
type: cloud-api
tags: [Localization]
---

# V1 / Country Regions

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/country-regions` | Get list of country regions sorted by localized name |

### `GET` `/v1/country-regions`

**Parameters:**

- `locale` (query, string) - 

**Responses:**

- `200` - OK
- `400` - 2: Invalid supported locale code.
- `403` - 7: Feature is disabled

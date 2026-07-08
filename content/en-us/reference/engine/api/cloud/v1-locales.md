---
title: V1 / Locales
type: cloud-api
tags: [Localization]
---

# V1 / Locales

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/locales` | Get list of Supported locales with user locus information. |

### `GET` `/v1/locales`

**Parameters:**

- `displayValueLocale` (query, string) - 

**Responses:**

- `200` - OK
- `403` - Feature is turned off temporary
- `500` - Internal server error

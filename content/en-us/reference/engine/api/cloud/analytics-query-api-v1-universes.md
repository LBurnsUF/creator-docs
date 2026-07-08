---
title: Analytics Query Api / V1 / Universes
type: cloud-api
tags: [Analytics]
---

# Analytics Query Api / V1 / Universes

Cloud API resource group with 4 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/analytics-query-api/v1/universes/{universeId}/dimension-values` | Queries dimension values for a universe. [BETA] |
| `POST` | `/analytics-query-api/v1/universes/{universeId}/metrics` | Queries time series metric data for a universe. [BETA] |
| `GET` | `/analytics-query-api/v1/universes/{universeId}/operations/dimension-values/{operationId}` | Retrieves the result of a long-running dimension values operation. [BETA] |
| `GET` | `/analytics-query-api/v1/universes/{universeId}/operations/metrics/{operationId}` | Retrieves the result of a long-running metrics query operation. [BETA] |

### `POST` `/analytics-query-api/v1/universes/{universeId}/dimension-values`

**Stability:** BETA

See the <a href="https://create.roblox.com/docs/cloud/guides/analytics">Analytics guide</a> for more information.

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID to query dimension values for.

**Request Body:** The dimension values request.

**Responses:**

- `200` - OK
- `202` - Accepted
- `400` - Bad Request
- `403` - Forbidden
- `429` - Too Many Requests
- `500` - Internal Server Error
- `503` - Service Unavailable
- `504` - Gateway Timeout

### `POST` `/analytics-query-api/v1/universes/{universeId}/metrics`

**Stability:** BETA

See the <a href="https://create.roblox.com/docs/cloud/guides/analytics">Analytics guide</a> for more information.

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID to query metrics for.

**Request Body:** The query request.

**Responses:**

- `200` - OK
- `202` - Accepted
- `400` - Bad Request
- `403` - Forbidden
- `429` - Too Many Requests
- `500` - Internal Server Error
- `503` - Service Unavailable
- `504` - Gateway Timeout

### `GET` `/analytics-query-api/v1/universes/{universeId}/operations/dimension-values/{operationId}`

**Stability:** BETA

See the <a href="https://create.roblox.com/docs/cloud/guides/analytics">Analytics guide</a> for more information.

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID the operation belongs to.
- `operationId` (path, string (required)) - The operation id returned from a prior dimension values request.

**Responses:**

- `200` - OK
- `202` - Accepted
- `400` - Bad Request
- `404` - Not Found
- `429` - Too Many Requests
- `500` - Internal Server Error
- `503` - Service Unavailable
- `504` - Gateway Timeout

### `GET` `/analytics-query-api/v1/universes/{universeId}/operations/metrics/{operationId}`

**Stability:** BETA

See the <a href="https://create.roblox.com/docs/cloud/guides/analytics">Analytics guide</a> for more information.

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID the operation belongs to.
- `operationId` (path, string (required)) - The operation id returned from a prior query request.

**Responses:**

- `200` - OK
- `202` - Accepted
- `400` - Bad Request
- `404` - Not Found
- `429` - Too Many Requests
- `500` - Internal Server Error
- `503` - Service Unavailable
- `504` - Gateway Timeout

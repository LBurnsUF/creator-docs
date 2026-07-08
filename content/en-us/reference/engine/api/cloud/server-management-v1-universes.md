---
title: Server Management / V1 / Universes
type: cloud-api
tags: [Places, Universes]
---

# Server Management / V1 / Universes

Cloud API resource group with 6 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/server-management/v1/universes/{universeId}/places/{placeId}/game-servers:filter-options` | Gets available filter options for game servers. [BETA] |
| `GET` | `/server-management/v1/universes/{universeId}/places/{placeId}/versions/{versionNumber}/game-servers` | Lists game servers for a specific place version. [BETA] |
| `GET` | `/server-management/v1/universes/{universeId}/places/{placeId}/versions/{versionNumber}/game-servers/{jobId}/logs` | Lists game server logs for a specific server job id [BETA] |
| `GET` | `/server-management/v1/universes/{universeId}/restarts` | List restart statuses for a universe. [BETA] |
| `POST` | `/server-management/v1/universes/{universeId}/restarts` | Launch a game server restart for a universe. [BETA] |
| `GET` | `/server-management/v1/universes/{universeId}/restarts:forecast` | Forecast the impact of restarting game servers for a universe. [BETA] |

### `GET` `/server-management/v1/universes/{universeId}/places/{placeId}/game-servers:filter-options`

**Operation:** `GameServers_GetFilterOptions`

**Stability:** BETA

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID
- `placeId` (path, integer (required)) - The place ID
- `Filter` (query) - The specific filter to query. If null or empty, the endpoint returns all available filters.

**Responses:**

- `200` - Success
- `400` - Bad Request
- `401` - Unauthorized
- `403` - Forbidden

### `GET` `/server-management/v1/universes/{universeId}/places/{placeId}/versions/{versionNumber}/game-servers`

**Operation:** `GameServers_ListGameServers`

**Stability:** BETA

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID
- `placeId` (path, integer (required)) - The place ID
- `versionNumber` (path, string (required)) - The version number
- `MaxPageSize` (query, integer) - The maximum number of game servers to return. The service might return fewer than this value. If unspecified, at most 25 game servers are returned. 
- `PageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page. When paginating, all other parameters provided to the subsequent call mus
- `OrderBy` (query, string) - Sorting is supported only for a single field at a time. Example: "orderBy": "uptime" Defaults to ascending, but descending ordering is also supporte
- `Filter` (query, string) - This field may be set in order to filter the resources returned. - CEL filtering is supported on all fields. - Supported operators &&, <, <=, >, >=,

**Responses:**

- `200` - Success
- `400` - Bad Request
- `401` - Unauthorized
- `403` - Forbidden

### `GET` `/server-management/v1/universes/{universeId}/places/{placeId}/versions/{versionNumber}/game-servers/{jobId}/logs`

**Operation:** `GameServers_ListGameServerLogs`

**Stability:** BETA

**Parameters:**

- `universeId` (path, integer (required)) - The universe id
- `placeId` (path, integer (required)) - The place id
- `versionNumber` (path, string (required)) - The version number
- `jobId` (path, string (required)) - The server job id
- `MaxPageSize` (query, integer) - The maximum number of game servers to return. The service might return fewer than this value. If unspecified, at most 25 game servers are returned. 
- `PageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page. When paginating, all other parameters provided to the subsequent call mus
- `OrderBy` (query, string) - Sorting is supported only for a single field at a time. Example: "orderBy": "uptime" Defaults to ascending, but descending ordering is also supporte
- `Filter` (query, string) - This field may be set in order to filter the resources returned. - CEL filtering is supported on all fields. - Supported operators &&, <, <=, >, >=,

**Responses:**

- `200` - Success
- `400` - Bad Request
- `401` - Unauthorized
- `403` - Forbidden

### `GET` `/server-management/v1/universes/{universeId}/restarts`

**Operation:** `Restarts_ListRestartStatuses`

**Stability:** BETA

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID

**Responses:**

- `200` - Success
- `400` - Bad Request
- `401` - Unauthorized
- `403` - Forbidden

### `POST` `/server-management/v1/universes/{universeId}/restarts`

**Operation:** `Restarts_LaunchRestart`

**Stability:** BETA

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID

**Request Body:** The launch restart request body

**Responses:**

- `200` - Success
- `400` - Bad Request
- `401` - Unauthorized
- `403` - Forbidden

### `GET` `/server-management/v1/universes/{universeId}/restarts:forecast`

**Operation:** `Restarts_ForecastRestart`

**Stability:** BETA

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID

**Responses:**

- `200` - Success
- `400` - Bad Request
- `401` - Unauthorized
- `403` - Forbidden

---
title: V1 / Translation Analytics / Games
type: cloud-api
tags: [Localization, Universes]
---

# V1 / Translation Analytics / Games

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/translation-analytics/games/{gameId}/download-translation-analytics-report` | Download translation analytics report after the report is ready |
| `POST` | `/v1/translation-analytics/games/{gameId}/request-translation-analytics-report` | Request translation analytics report to be generated |

### `GET` `/v1/translation-analytics/games/{gameId}/download-translation-analytics-report`

**Parameters:**

- `gameId` (path, integer (required)) - The game's id
- `startDateTime` (query, string (required)) - The inclusive start dateTime of report in UTC
- `endDateTime` (query, string (required)) - The exclusive end dateTime of report in UTC
- `reportType` (query, string (required)) - The report type
- `reportSubjectTargetId` (query, integer (required)) - The translator group id

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id 56: You need to provide a valid translator group id to get report. 58: Start d
- `401` - 0: Authorization has been denied for this request.
- `403` - 57: You do not have permission to request translation analytics report.

### `POST` `/v1/translation-analytics/games/{gameId}/request-translation-analytics-report`

**Parameters:**

- `gameId` (path, integer (required)) - The game's id

**Request Body:** The request body

**Responses:**

- `200` - OK
- `400` - 14: Invalid game id 56: You need to provide a valid translator group id to get report. 58: Start d
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 57: You do not have permission to request translation analytics report.

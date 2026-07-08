---
title: V1 / Universe Payout History
type: cloud-api
tags: [Universes]
---

# V1 / Universe Payout History

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/universe-payout-history` | Gets the engagement payout history for a specific universe and a given date range, specified by star |

### `GET` `/v1/universe-payout-history`

**Parameters:**

- `universeId` (query, integer (required)) - The ID of the universe in question.
- `startDate` (query, string (required)) - The first date in the range, specified as yyyy-MM-dd.
- `endDate` (query, string (required)) - The last date in the range, specified as yyyy-MM-dd.

**Responses:**

- `200` - OK
- `400` - 1: InvalidUniverseId 2: InvalidStartDate 3: InvalidEndDate 4: InvalidDateRange 5: Forbidden 6: 
- `401` - 0: Authorization has been denied for this request.

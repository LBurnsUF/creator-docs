---
title: V1 / Display Names / Validate
type: cloud-api
tags: [Users]
---

# V1 / Display Names / Validate

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/display-names/validate` | Validate a display name for a new user. |

### `GET` `/v1/display-names/validate`

**Parameters:**

- `displayName` (query, string (required)) - The display name.
- `birthdate` (query, string (required)) - The new user's birthdate

**Responses:**

- `200` - OK
- `400` - 1: Display name is too short 2: Display name is too long 3: Display name contains invalid characte
- `429` - 5: Display name updates for this user have been throttled

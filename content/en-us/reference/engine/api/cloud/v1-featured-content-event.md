---
title: V1 / Featured Content / Event
type: cloud-api
tags: [Groups]
---

# V1 / Featured Content / Event

Cloud API resource group with 3 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `DELETE` | `/v1/featured-content/event` | Deletes the featured event for a group |
| `GET` | `/v1/featured-content/event` | Gets the featured event for a group |
| `POST` | `/v1/featured-content/event` | Sets the featured event for a group |

### `DELETE` `/v1/featured-content/event`

**Parameters:**

- `groupId` (query, integer (required)) - The group Id.
- `eventId` (query, integer (required)) - The event Id.

**Responses:**

- `200` - OK
- `403` - 0: Token Validation Failed 3: User is not authorized to set featured content for this group.

### `GET` `/v1/featured-content/event`

**Parameters:**

- `groupId` (query, integer (required)) - The group Id.

**Responses:**

- `200` - OK

### `POST` `/v1/featured-content/event`

**Parameters:**

- `groupId` (query, integer (required)) - The group Id.
- `eventId` (query, integer (required)) - The event Id.

**Responses:**

- `200` - OK
- `403` - 0: Token Validation Failed 3: User is not authorized to set featured content for this group.

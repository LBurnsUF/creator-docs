---
title: V1 / Vip Servers
type: cloud-api
tags: [Groups, Metadata, Private servers, Universes]
---

# V1 / Vip Servers

Cloud API resource group with 4 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/vip-servers/{id}` |  |
| `PATCH` | `/v1/vip-servers/{id}` |  |
| `PATCH` | `/v1/vip-servers/{id}/permissions` |  |
| `PATCH` | `/v1/vip-servers/{id}/subscription` |  |

### `GET` `/v1/vip-servers/{id}`

**Operation:** `PrivateServers_GetPrivateServer`

**Parameters:**

- `id` (path, integer (required)) - 

**Responses:**

- `200` - Success

### `PATCH` `/v1/vip-servers/{id}`

**Operation:** `PrivateServers_UpdatePrivateServer`

**Parameters:**

- `id` (path, integer (required)) - 

**Responses:**

- `200` - Success

### `PATCH` `/v1/vip-servers/{id}/permissions`

**Operation:** `PrivateServers_UpdatePrivateServerPermissions`

**Parameters:**

- `id` (path, integer (required)) - 

**Responses:**

- `200` - Success

### `PATCH` `/v1/vip-servers/{id}/subscription`

**Operation:** `PrivateServers_UpdatePrivateServerSubscription`

**Parameters:**

- `id` (path, integer (required)) - 

**Responses:**

- `200` - Success

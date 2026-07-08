---
title: Assets / V1 / Operations
type: cloud-api
tags: [Assets]
---

# Assets / V1 / Operations

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/assets/v1/operations/{operationId}` | Get the result of an asset creation or update. [BETA] |

### `GET` `/assets/v1/operations/{operationId}`

**Operation:** `Assets_GetOperation`

**Stability:** BETA

Get the result of an asset creation or update using the returned Operation ID. Requires **Read** for the API key permission and **asset:read** for OAuth 2.0 apps.

**Parameters:**

- `operationId` (path, string (required)) - The unique identifier of the operation.

**Responses:**

- `200` - Operation result retrieved successfully.
- `400` - Invalid argument. Failed to parse the request or the file.
- `401` - The API key is not valid for this operation / You don't have the authorization.
- `500` - Server internal error / Unknown error.

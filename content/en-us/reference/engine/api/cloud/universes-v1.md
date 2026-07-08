---
title: Universes / V1
type: cloud-api
tags: [Places, Universes]
---

# Universes / V1

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/universes/v1/{universeId}/places/{placeId}/versions` | Publish a new place or update an existing place with a new version. Provide a RBXL or RBXLX file in  [BETA] |

### `POST` `/universes/v1/{universeId}/places/{placeId}/versions`

**Operation:** `Places_CreatePlaceVersionApiKey`

**Stability:** BETA

Publish a new place or update an existing place with a new version. Provide a RBXL or RBXLX file in the data-binary.

**Parameters:**

- `universeId` (path, integer (required)) - The identifier of the experience in which you want to publish your place to. You can [copy your experience's Universe ID](/cloud/guides/usage-place-pu
- `placeId` (path, integer (required)) - The identifier of your place. See [Publishing places with API keys](/cloud/guides/usage-place-publishing.md) on obtaining a Place ID.
- `versionType` (query, string) - Can only be either:  - `Saved`: the place file should be saved, but not published.   - `Published`: the place file should be saved and published.

**Responses:**

- `200` - Returns the published place's version number.
- `400` - Invalid request / Invalid file content.
- `401` - API key not valid for operation, user does not have authorization.
- `403` - Publish not allowed on place.
- `404` - Place or universe does not exist.
- `409` - Place not part of the universe.
- `500` - Server internal error / Unknown error.

---
title: Legacy Publish / V1 / Badges
type: cloud-api
tags: [Assets, Badges, Thumbnails]
---

# Legacy Publish / V1 / Badges

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/legacy-publish/v1/badges/{badgeId}/icon` | Overwrites a badge icon with a new one. |

### `POST` `/legacy-publish/v1/badges/{badgeId}/icon`

**Parameters:**

- `badgeId` (path, integer (required)) - The badge Id.

**Responses:**

- `200` - OK
- `400` - 2: File not present in request. 12: Name or description is moderated.
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed 5: You do not have permission to manage this item.
- `404` - 4: Target item is invalid or does not exist.
- `429` - 3: You're uploading too much, please wait and try again later.

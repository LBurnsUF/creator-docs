---
title: V1 / Audio
type: cloud-api
tags: [Assets]
---

# V1 / Audio

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/audio` | Published an audio file and returns the new asset info. |

### `POST` `/v1/audio`

**Request Body:** The file upload request body. Roblox.Publish.Api.UploadAudioRequest

**Responses:**

- `200` - OK
- `400` - 3: The request did not contain a file to be uploaded. 4: The file in the request is too large. 5: 
- `401` - 0: Authorization has been denied for this request. 1: The request did not include an authorization.
- `403` - 0: Token Validation Failed
- `500` - 19: Asset creation was unavailable. Please try again.

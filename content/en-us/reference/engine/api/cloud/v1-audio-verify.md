---
title: V1 / Audio / Verify
type: cloud-api
tags: [Assets]
---

# V1 / Audio / Verify

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/audio/verify` | Verifies an audio file and returns a product that you can purchase to publish the audio file. |

### `POST` `/v1/audio/verify`

**Request Body:** The verify audio request body. Roblox.Publish.Api.VerifyAudioRequest

**Responses:**

- `200` - OK
- `400` - 3: The request did not contain a file to be uploaded. 4: The file in the request is too large. 5: 
- `401` - 0: Authorization has been denied for this request. 1: The request did not include an authorization.
- `403` - 0: Token Validation Failed

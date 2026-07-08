---
title: Messaging Service / V1 / Universes
type: cloud-api
tags: [Universes]
---

# Messaging Service / V1 / Universes

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/messaging-service/v1/universes/{universeId}/topics/{topic}` | Publish a cross-server message to a universe [BETA] |

### `POST` `/messaging-service/v1/universes/{universeId}/topics/{topic}`

**Operation:** `CrossServerMessaging_Publish`

**Stability:** BETA

Publish a message to a pre-defined topic of an experience, with the size of the message up to 1,024 characters (1 KB). Requires the **Publish** permission for API keys and the **universe-messaging-service:publish** scope for OAuth 2.0 apps. See [Cross-server messaging](/cloud-services/cross-server-messaging.md#subscribe-users-to-receive-messages) for defining and subscribing users to a topic.

**Parameters:**

- `universeId` (path, integer (required)) - The identifier of the experience in which you want to send your messages to. You can [copy your experience's Universe ID](/cloud/guides/usage-messagin
- `topic` (path, string (required)) - The topic that you want to publish your message to, with up to 80 characters.

**Responses:**

- `200` - Returns an empty response body.
- `400` - Invalid request.
- `401` - The API key is not valid for this operation / You don't have the authorization.
- `403` - Publishing is not allowed on this experience.
- `500` - Server internal error / Unknown error.

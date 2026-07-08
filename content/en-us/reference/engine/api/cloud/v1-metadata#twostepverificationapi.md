---
title: V1 / Metadata#Twostepverificationapi
type: cloud-api
tags: [Accounts, Metadata]
---

# V1 / Metadata#Twostepverificationapi

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/metadata#TwoStepVerificationApi` | Gets two step verification system metadata. |

### `GET` `/v1/metadata#TwoStepVerificationApi`

The metadata endpoint takes in optional request parameters to output additional context
for when the user is unauthenticated but attempting to login with two step verification.

When supplied, all three request parameters must be sent and match up.

**Parameters:**

- `userId` (query, integer) - The user ID.
- `challengeId` (query, string) - The active two step verification challenge ID if there is one.
- `actionType` (query, integer) - The Roblox.TwoStepVerification.Client.TwoStepVerificationActionType associated with the challenge.

**Responses:**

- `200` - OK

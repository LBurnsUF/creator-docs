---
title: V2 / Push Notifications / Deregister Current Device
type: cloud-api
tags: [Notifications]
---

# V2 / Push Notifications / Deregister Current Device

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v2/push-notifications/deregister-current-device` | De-register current device to disable push notifications |

### `POST` `/v2/push-notifications/deregister-current-device`

**Responses:**

- `200` - OK
- `401` - 0: Authorization has been denied for this request.
- `403` - 0: Token Validation Failed

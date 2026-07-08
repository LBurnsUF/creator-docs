---
title: V1 / Usernames / Users
type: cloud-api
tags: [Users]
---

# V1 / Usernames / Users

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/v1/usernames/users` | Get users by usernames. |

### `POST` `/v1/usernames/users`

This endpoint will also check previous usernames.
Does not require X-CSRF-Token protection because this is essentially a get request but as a POST to avoid URI limits.

**Request Body:** The Roblox.Users.Api.MultiGetByUsernameRequest.

**Responses:**

- `200` - OK
- `400` - 2: Too many usernames.

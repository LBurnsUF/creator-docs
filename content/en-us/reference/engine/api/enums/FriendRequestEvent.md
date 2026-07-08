---
title: FriendRequestEvent
type: enum
---

# `Enum.FriendRequestEvent`

Describes the event when a player sends or responds to a friend request. This
is used by the in-game friend request system.

The `Enum.FriendRequestEvent` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.FriendRequestEvent.Issue` | 0 | A player invokes (sends) a friend request. |
| `Enum.FriendRequestEvent.Revoke` | 1 | A player revokes (cancels) a previously invoked (sent) friend request. |
| `Enum.FriendRequestEvent.Accept` | 2 | A player accepts a friend request. |
| `Enum.FriendRequestEvent.Deny` | 3 | A player denies a friend request. |

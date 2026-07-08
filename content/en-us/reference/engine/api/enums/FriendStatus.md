---
title: FriendStatus
type: enum
---

# `Enum.FriendStatus`

Determines the friend status between two players. This is used by the in-game
friend request system.

The `Enum.FriendStatus` enum has 5 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.FriendStatus.Unknown` | 0 | The friend status of two players is unknown. |
| `Enum.FriendStatus.NotFriend` | 1 | Two players are not friends. |
| `Enum.FriendStatus.Friend` | 2 | Two players are friends. |
| `Enum.FriendStatus.FriendRequestSent` | 3 | At least one of two players has sent a friend request to the other player. |
| `Enum.FriendStatus.FriendRequestReceived` | 4 | At least one of two players has received a friend request sent by the other player. |

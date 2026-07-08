---
title: PlayerExitReason
type: enum
---

# `Enum.PlayerExitReason`

An enum that specifies the reason for **Players.PlayerRemoving** signal.

Second argument in `Class.Players.PlayerRemoving`. Helps identify whether a
kick was caused by the Roblox platform or the Creator.

The `Enum.PlayerExitReason` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.PlayerExitReason.Unknown` | 0 | Catch-all for all other disconnect reasons. |
| `Enum.PlayerExitReason.PlatformKick` | 1 | User was kicked by Roblox systems, such as being blocked while in a Private Server. |
| `Enum.PlayerExitReason.CreatorKick` | 2 | Creator called **Player:Kick()** |

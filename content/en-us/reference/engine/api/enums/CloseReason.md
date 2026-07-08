---
title: CloseReason
type: enum
---

# `Enum.CloseReason`

Specifies the reason for the experience server shutdown.

Specifies the reason for the experience server shutdown. This enum value is
the first parameter passed to functions bound by
`Class.DataModel:BindToClose()|BindToClose()`.

The **DeveloperShutdown** value must always be passed to functions bound by
`Class.DataModel:BindToClose()|BindToClose()` when they're called in Studio.

The `Enum.CloseReason` enum has 7 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.CloseReason.Unknown` | 0 | The server shut down for an unknown reason. |
| `Enum.CloseReason.RobloxMaintenance` | 1 | The server shut down for maintenance. |
| `Enum.CloseReason.DeveloperShutdown` | 2 | The experience developer has shut down the server, or functions bound by `Class.DataModel:BindToClos |
| `Enum.CloseReason.DeveloperUpdate` | 3 | The experience developer has migrated the server to a new place version. |
| `Enum.CloseReason.ServerEmpty` | 4 | The last player has left and the experience is empty. |
| `Enum.CloseReason.OutOfMemory` | 5 | The experience has hit the memory limit for the game server. |
| `Enum.CloseReason.Moderation` | 6 |  |

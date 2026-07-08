---
title: TeleportState
type: enum
---

# `Enum.TeleportState`

Determines the current teleportation state of a player.

Determines the current teleportation state of a player.

The `Enum.TeleportState` enum has 5 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.TeleportState.RequestedFromServer` | 0 | The server has requested that the client teleport. |
| `Enum.TeleportState.Started` | 1 | The client has started attempting to teleport. |
| `Enum.TeleportState.WaitingForServer` | 2 | The client is waiting for the server to respond to the teleport request. |
| `Enum.TeleportState.Failed` | 3 | The teleport failed. |
| `Enum.TeleportState.InProgress` | 4 | The teleport is currently in progress. The player usually disconnects and teleports to the destinati |

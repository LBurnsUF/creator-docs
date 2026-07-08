---
title: TeleportResult
type: enum
---

# `Enum.TeleportResult`

Describes the result of a teleport.

Describes the result of a teleport.

The `Enum.TeleportResult` enum has 8 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.TeleportResult.Success` | 0 | The teleport was successful. |
| `Enum.TeleportResult.Failure` | 1 | The teleport failed for an unknown reason. |
| `Enum.TeleportResult.GameNotFound` | 2 | The game that this player attempted to teleport to could not be found. |
| `Enum.TeleportResult.GameEnded` | 3 | The game that this player attempted to teleport to has ended. |
| `Enum.TeleportResult.GameFull` | 4 | The game that this player attempted to teleport to is full. |
| `Enum.TeleportResult.Unauthorized` | 5 | The player is not authorized to complete this teleport. |
| `Enum.TeleportResult.Flooded` | 6 | Too many teleport requests have been made recently. |
| `Enum.TeleportResult.IsTeleporting` | 7 | The player is currently being teleported. |

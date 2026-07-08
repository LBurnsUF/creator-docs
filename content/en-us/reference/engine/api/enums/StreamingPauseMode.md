---
title: StreamingPauseMode
type: enum
---

# `Enum.StreamingPauseMode`

Determines how a client should handle not having enough content streamed in to
continue playing properly.

This enum is used to control `Class.Workspace.StreamingPauseMode` behavior.
The `Disabled` mode indicates that gameplay continues unchanged even if player
does not have the minimum streaming radius available. In `ClientPhysicsPause`
mode, client-side physics is paused when the player doesn't have the minimum
radius present and resumed when the minimum radius is available.

The `Enum.StreamingPauseMode` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.StreamingPauseMode.Default` | 0 | Default behavior (subject to change). |
| `Enum.StreamingPauseMode.Disabled` | 1 | No change to gameplay due to streaming region availability. |
| `Enum.StreamingPauseMode.ClientPhysicsPause` | 2 | Client owned physics is paused. |

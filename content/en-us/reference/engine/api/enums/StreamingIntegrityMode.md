---
title: StreamingIntegrityMode
type: enum
---

# `Enum.StreamingIntegrityMode`

Determines how a user's client should handle not having enough content
streamed in.

This enum is used to control `Class.Workspace.StreamingIntegrityMode`
behavior. For all modes, the replication focus defaults to be the local
character model unless explicitly set via `Class.Player.ReplicationFocus`.

Note that `MinimumRadiusPause` and `PauseOutsideLoadedArea` both set the
`Class.Player.GameplayPaused` property when their respective pause logic is
triggered, and a default message is displayed on the client.

The `Enum.StreamingIntegrityMode` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.StreamingIntegrityMode.Default` | 0 | Default behavior (subject to change). |
| `Enum.StreamingIntegrityMode.Disabled` | 1 | Simulation of the replication focus is never paused, regardless of the amount of content streamed in |
| `Enum.StreamingIntegrityMode.MinimumRadiusPause` | 2 | All client-side simulation is paused when content is not streamed in up to the minimum radius. |
| `Enum.StreamingIntegrityMode.PauseOutsideLoadedArea` | 3 | Simulation of the replication focus is paused when any part of its bounding box is not in a streamed |

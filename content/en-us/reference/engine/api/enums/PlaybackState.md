---
title: PlaybackState
type: enum
---

# `Enum.PlaybackState`

Describes the current state of a `Class.Tween` in its
`Class.Tween.PlaybackState` property.

Describes the current state of a `Class.Tween` in its
`Class.Tween.PlaybackState` property.

The `Enum.PlaybackState` enum has 6 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.PlaybackState.Begin` | 0 | The tween has been created, but has yet to be played. After exiting this state, the tween never ente |
| `Enum.PlaybackState.Delayed` | 1 | The tween is waiting for the duration specified in its `Datatype.TweenInfo.DelayTime`. After the del |
| `Enum.PlaybackState.Playing` | 2 | The tween is currently in progress. |
| `Enum.PlaybackState.Paused` | 3 | The tween is paused in the middle of playing. |
| `Enum.PlaybackState.Completed` | 4 | The tween completed successfully. |
| `Enum.PlaybackState.Cancelled` | 5 | The tween was cancelled before completion. |

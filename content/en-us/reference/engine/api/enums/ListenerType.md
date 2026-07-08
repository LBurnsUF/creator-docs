---
title: ListenerType
type: enum
---

# `Enum.ListenerType`

Defines where and how the listener is positioned when picking up spatial
audio.

Defines where and how the listener is positioned when picking up spatial
audio. Used in `Class.SoundService.SetListener` and
`Class.SoundService.GetListener`.

The `Enum.ListenerType` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ListenerType.Camera` | 0 | Uses the world CFrame of `workspace.CurrentCamera`. |
| `Enum.ListenerType.CFrame` | 1 | Uses a specified world CFrame. |
| `Enum.ListenerType.ObjectPosition` | 2 | Uses the world position of an instance and the rotation of `workspace.CurrentCamera`. |
| `Enum.ListenerType.ObjectCFrame` | 3 | Uses the world CFrame from an instance. |

---
title: ListenerLocation
type: enum
---

# `Enum.ListenerLocation`

Enum used with `Class.SoundService.DefaultListenerLocation` to determine where
an `Class.AudioListener` is placed by default.

Enum used with `Class.SoundService.DefaultListenerLocation` to determine where
an `Class.AudioListener` is placed by default.

The `Enum.ListenerLocation` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ListenerLocation.Default` | 0 | Behavior depends on the value of `Class.VoiceChatService.EnableDefaultVoice` and `Class.VoiceChatSer |
| `Enum.ListenerLocation.None` | 1 | No `Class.AudioListener` will be created by default, but they can be created separately by scripts. |
| `Enum.ListenerLocation.Character` | 2 | All of the following, resulting in the world being heard from the position of your character while m |
| `Enum.ListenerLocation.Camera` | 3 | All of the following, resulting in the world being heard from the perspective (postition and orienta |

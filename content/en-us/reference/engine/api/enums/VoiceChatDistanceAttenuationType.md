---
title: VoiceChatDistanceAttenuationType
type: enum
---

# `Enum.VoiceChatDistanceAttenuationType`

Enum used for preset distance attenuation curve options in the default voice
chat setup.

Each value in this enum represents a distance attenuation curve that can be
used by `Class.VoiceChatService` when creating the default voice chat setup
using `Class.AudioDeviceInput` and `Class.AudioEmitter` objects.

The `Enum.VoiceChatDistanceAttenuationType` enum has 2 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.VoiceChatDistanceAttenuationType.Inverse` | 0 | Represents a distance attenuation curve that follows the inverse-squared law. This is identical to t |
| `Enum.VoiceChatDistanceAttenuationType.Legacy` | 1 | Represents a linear-squared distance attenuation curve with a minimum distance of `7` and a maximum  |

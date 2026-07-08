---
title: AudioApiRollout
type: enum
---

# `Enum.AudioApiRollout`

Used to determine whether voice chat is represented and controlled by
`Class.AudioDeviceInput` objects.

Used to determine whether voice chat is represented and controlled by
`Class.AudioDeviceInput` objects.

The `Enum.AudioApiRollout` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.AudioApiRollout.Disabled` | 0 | Voice chat will use an internal voice chat implementation that is automatic and hidden. |
| `Enum.AudioApiRollout.Automatic` | 1 | Currently means the same thing as `Disabled`, but will be updated to mean `Enabled` in the future. |
| `Enum.AudioApiRollout.Enabled` | 2 | Voice chat can be customized or controlled via `Class.AudioDeviceInput/AudioDeviceInputs`. |

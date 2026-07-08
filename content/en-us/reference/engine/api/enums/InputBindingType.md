---
title: InputBindingType
type: enum
---

# `Enum.InputBindingType`

This enum is used by `Class.InputBinding.Type` to determine whether the
binding responds to hardware input or is driven programmatically.

This enum is used by `Class.InputBinding.Type` to determine whether the
`Class.InputBinding` responds to hardware input devices or is driven
programmatically via `Class.InputBinding:Fire()`.

The `Enum.InputBindingType` enum has 2 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.InputBindingType.Automatic` | 0 | The `Class.InputBinding` responds to physical input devices (keyboard, mouse, gamepad, touch) based  |
| `Enum.InputBindingType.Scriptable` | 1 | The `Class.InputBinding` ignores hardware input and instead receives state updates exclusively throu |

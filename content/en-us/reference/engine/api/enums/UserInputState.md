---
title: UserInputState
type: enum
---

# `Enum.UserInputState`

This enum describes the state of an input that is currently or was recently
performed.

The `UserInputState` enum describes the state of an input that is currently or
was recently performed. It is used by the `Class.InputObject.UserInputState`
property of the same name, as well as various `Class.UserInputService` and
`Class.GuiObject` events.

Depending on the `Enum.UserInputType`, input may follow states differently:

- Simple button and key presses generally follow a simple `Begin` to `End`
  flow. Analog gamepad trigger buttons are similar to button presses but will
  use `Change` as the trigger pressure changes.
- Mouse movement generally follows `Begin` (mouse-over) to `Change` (mouse
  movement) to `End` (mouse-leave).
- Touch input behaves somewhat similarly to mouse movement. `Begin` and `End`
  occur when the user starts or ends touching the screen, respectively. The
  same `Class.InputObject` is used for the same touch point.
- Gamepad thumbstick controls will cause `Change` to occur each frame the
  position changes.

The `Enum.UserInputState` enum has 5 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.UserInputState.Begin` | 0 | Occurs when an `Class.InputObject` starts to interact with the experience. For example, a mouse butt |
| `Enum.UserInputState.Change` | 1 | Occurs each frame an `Class.InputObject` has already begun interacting with the experience and part  |
| `Enum.UserInputState.End` | 2 | Occurs when an `Class.InputObject` finishes interacting with the experience. For example, a mouse bu |
| `Enum.UserInputState.Cancel` | 3 | A special circumstance state that indicates this input is no longer relevant, particularly with `Cla |
| `Enum.UserInputState.None` | 4 | A state that should never be seen in an experience; essentially just marks the end of the enum. |

---
title: UserInputType
type: enum
---

# `Enum.UserInputType`

Describes the type of a user input event.

The **UserInputType** enum describes the kind of input being performed (mouse,
keyboard, gamepad, touch, etc). This enum is used by the
`Class.InputObject.UserInputType` property of the same name, as well as
various `Class.UserInputService` and `Class.GuiObject` events.

The `Enum.UserInputType` enum has 21 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.UserInputType.MouseButton1` | 0 | The left mouse button. |
| `Enum.UserInputType.MouseButton2` | 1 | The right mouse button. |
| `Enum.UserInputType.MouseButton3` | 2 | The middle mouse button. |
| `Enum.UserInputType.MouseWheel` | 3 | The mouse wheel. |
| `Enum.UserInputType.MouseMovement` | 4 | Movement of the mouse. Fires changed events each time the player's cursor position changes and when  |
| `Enum.UserInputType.Touch` | 7 | A tap on the screen from a mobile device. |
| `Enum.UserInputType.Keyboard` | 8 | Key press on a keyboard. |
| `Enum.UserInputType.Focus` | 9 | The client regaining focus of the Roblox window. |
| `Enum.UserInputType.Accelerometer` | 10 | The accelerometer of a mobile device. |
| `Enum.UserInputType.Gyro` | 11 | The Gyroscope of a mobile device. |
| `Enum.UserInputType.Gamepad1` | 12 | Input from the 1st plugged in Gamepad. |
| `Enum.UserInputType.Gamepad2` | 13 | Input from the 2nd plugged in Gamepad. |
| `Enum.UserInputType.Gamepad3` | 14 | Input from the 3rd plugged in Gamepad. |
| `Enum.UserInputType.Gamepad4` | 15 | Input from the 4th plugged in Gamepad. |
| `Enum.UserInputType.Gamepad5` | 16 | Input from the 5th plugged in Gamepad. |
| `Enum.UserInputType.Gamepad6` | 17 | Input from the 6th plugged in Gamepad. |
| `Enum.UserInputType.Gamepad7` | 18 | Input from the 7th plugged in Gamepad. |
| `Enum.UserInputType.Gamepad8` | 19 | Input from the 8th plugged in Gamepad. |
| `Enum.UserInputType.TextInput` | 20 | Input of Text into a text-based `Class.GuiObject`. Normally this is only a `Class.TextBox`. |
| `Enum.UserInputType.InputMethod` | 21 | Text input from an input method editor (IME). `Class.InputObject/InputObjects` with this type aren't |
| `Enum.UserInputType.None` | 22 | Unknown UserInputType. |

---
title: CameraMode
type: enum
---

# `Enum.CameraMode`

Used to set `Class.Player.CameraMode` to determine when first person and third
person cameras should be used.

The **CameraMode** enum is used to set `Class.Player.CameraMode` to determine
when first person and third person cameras should be used.

#### Third Person

In the default third person mode (`Enum.CameraMode|Classic`), the character
can be seen in the camera. While in this mode, the default behavior is:

- Players can right-click and drag (mouse), tap and drag (mobile), use the
  secondary thumbstick (gamepad), or press the left/right arrows (keyboard) to
  rotate the camera around their character.
- When a player moves their character, it faces in the corresponding movement
  direction.
- Players can zoom in and out freely, even to first person on full zoom in.

#### First Person

In first person mode (`Enum.CameraMode|LockFirstPerson`), the player's camera
is zoomed all the way in. Unless there is a visible GUI present with the
`Class.GuiButton.Modal` property set to `true`, moving the mouse, tap-dragging
on mobile, or using the secondary thumbstick on a gamepad will rotate the
camera around the character.

The `Enum.CameraMode` enum has 2 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.CameraMode.Classic` | 0 | Third person camera which can be zoomed into first person. |
| `Enum.CameraMode.LockFirstPerson` | 1 | Exclusively first person camera. |

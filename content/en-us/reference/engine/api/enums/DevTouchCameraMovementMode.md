---
title: DevTouchCameraMovementMode
type: enum
---

# `Enum.DevTouchCameraMovementMode`

Overwrites the camera mode if the player is on a touch device.

Overwrites the camera mode if the player is on a touch device.

The `Enum.DevTouchCameraMovementMode` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.DevTouchCameraMovementMode.UserChoice` | 0 | The camera will move based on the player's settings. |
| `Enum.DevTouchCameraMovementMode.Classic` | 1 | Camera tracks the player but will not automatically rotate if the player walks left or right. |
| `Enum.DevTouchCameraMovementMode.Follow` | 2 | Camera tracks the player and automatically rotates if the player walks left or right. |
| `Enum.DevTouchCameraMovementMode.Orbital` | 3 | The camera has a fixed Y position, but can be rotated around the player. |

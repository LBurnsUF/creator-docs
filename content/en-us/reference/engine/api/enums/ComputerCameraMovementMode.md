---
title: ComputerCameraMovementMode
type: enum
---

# `Enum.ComputerCameraMovementMode`

The camera movement mode currently in-use by the client.

The camera movement mode currently in-use by the client.

The `Enum.ComputerCameraMovementMode` enum has 5 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ComputerCameraMovementMode.Default` | 0 | The default camera movement mode is classic. |
| `Enum.ComputerCameraMovementMode.Classic` | 1 | Camera tracks the player but will not automatically rotate if the player walks left or right. |
| `Enum.ComputerCameraMovementMode.Follow` | 2 | Camera tracks the player and automatically rotates if the player walks left or right. |
| `Enum.ComputerCameraMovementMode.Orbital` | 3 | The camera has a fixed Y position, but can be rotated around the player. |
| `Enum.ComputerCameraMovementMode.CameraToggle` | 4 | The camera toggles between locked and free rotation with the right mouse button. |

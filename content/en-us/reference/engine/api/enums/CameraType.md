---
title: CameraType
type: enum
---

# `Enum.CameraType`

Describes the camera behavior mode if using the default PlayerScripts.

The CameraType Enum is used in `Class.Camera.CameraType` to set the behavior
of the Camera object.

Attach, Watch, Track, and Follow all require a valid
`Class.Camera.CameraSubject` to work properly.

The `Enum.CameraType` enum has 8 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.CameraType.Fixed` | 0 | Camera is stationary. |
| `Enum.CameraType.Attach` | 1 | Camera moves with the subject at a fixed offset and will rotate as the subject rotates. |
| `Enum.CameraType.Watch` | 2 | Camera is stationary but will rotate to keep the subject in the center of the screen. |
| `Enum.CameraType.Track` | 3 | Camera moves with the subject but does not rotate automatically. |
| `Enum.CameraType.Follow` | 4 | Camera moves with the subject and rotates to keep the subject in the center. |
| `Enum.CameraType.Custom` | 5 | Default mode used by Roblox core scripts. |
| `Enum.CameraType.Scriptable` | 6 | No default behavior. Used when developers need to script custom behavior. |
| `Enum.CameraType.Orbital` | 7 | The camera has a fixed Y position, but can be rotated around the player. |

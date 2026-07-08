---
title: Camera
type: class
superclass: PVInstance
tags: [NotReplicated]
---

# Camera

A class which defines a view of the 3D world.

**Inherits from:** `Class.PVInstance` > `Class.Instance` > `Class.Object`

**Tags:** [NotReplicated]

## Description

The `Camera` object defines a view of the 3D world. In a running experience,
each client has its own `Camera` object which resides in that client's local
`Class.Workspace`, accessible through the `Class.Workspace.CurrentCamera`
property.

The most important camera properties are:

- `Class.Camera.CFrame|CFrame` which represents the position and orientation
  of the camera.

- `Class.Camera.CameraType|CameraType` which is read by the experience's
  camera scripts and determines how the camera should update each frame.

- `Class.Camera.CameraSubject|CameraSubject` which is read by the experience's
  camera scripts and determines what object the camera should follow.

- `Class.Camera.FieldOfView|FieldOfView` which represents the visible extent
  of the observable world.

- `Class.Camera.Focus|Focus` which represents the point the camera is looking
  at. It's important this property is set, as certain visuals will be more
  detailed and will update more frequently depending on how close they are to
  the focus point.

See [Customizing the Camera](../../../workspace/camera.md) for more
information on how to adjust and customize the camera's behavior.

#### Storing Multiple Cameras

Note that when changing `Class.Workspace.CurrentCamera` to a new
`Class.Camera`, all other `Class.Camera|Cameras` directly descending from
`Class.Workspace` will be destroyed. If you need to store multiple cameras and
swap between them on demand, it's recommended that you store them in a
`Class.Folder` or `Class.Model` under `Class.Workspace`, inside which they
will remain even when `Class.Workspace.CurrentCamera|CurrentCamera` is
changed.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Camera.CFrame` | `Datatype.CFrame` |  |
| `Class.Camera.CameraSubject` | `Class.Instance` |  |
| `Class.Camera.CameraType` | `Enum.CameraType` |  |
| `Class.Camera.CoordinateFrame` | `Datatype.CFrame` | [Hidden] [NotReplicated] [Deprecated] |
| `Class.Camera.DiagonalFieldOfView` | `float` | [NotReplicated] |
| `Class.Camera.FieldOfView` | `float` |  |
| `Class.Camera.FieldOfViewMode` | `Enum.FieldOfViewMode` |  |
| `Class.Camera.Focus` | `Datatype.CFrame` |  |
| `Class.Camera.HeadLocked` | `bool` |  |
| `Class.Camera.HeadScale` | `float` |  |
| `Class.Camera.MaxAxisFieldOfView` | `float` | [NotReplicated] |
| `Class.Camera.NearPlaneZ` | `float` | [ReadOnly] [NotReplicated] |
| `Class.Camera.VRTiltAndRollEnabled` | `bool` |  |
| `Class.Camera.ViewportSize` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] |
| `Class.Camera.focus` | `Datatype.CFrame` | [NotReplicated] [Deprecated] |

## Methods

### `Class.Camera:GetLargestCutoffDistance`

``GetLargestCutoffDistance(ignoreList: `Datatype.Instances`)`` -> `float`
  [Deprecated]

### `Class.Camera:GetPanSpeed`

``GetPanSpeed()`` -> `float`
  [Deprecated]

### `Class.Camera:GetPartsObscuringTarget`

``GetPartsObscuringTarget(castPoints: `Array`, ignoreList: `Datatype.Instances`)`` -> `Datatype.Instances`

### `Class.Camera:GetRenderCFrame`

``GetRenderCFrame()`` -> `Datatype.CFrame`

### `Class.Camera:GetRoll`

``GetRoll()`` -> `float`

### `Class.Camera:GetTiltSpeed`

``GetTiltSpeed()`` -> `float`
  [Deprecated]

### `Class.Camera:Interpolate`

``Interpolate(endPos: `Datatype.CFrame`, endFocus: `Datatype.CFrame`, duration: `float`)`` -> `null`
  [Deprecated]

### `Class.Camera:PanUnits`

``PanUnits(units: `int`)`` -> `null`
  [Deprecated]

### `Class.Camera:ScreenPointToRay`

``ScreenPointToRay(x: `float`, y: `float`, depth: `float`)`` -> `Datatype.Ray`

### `Class.Camera:SetCameraPanMode`

``SetCameraPanMode(mode: `Enum.CameraPanMode`)`` -> `null`
  [Deprecated]

### `Class.Camera:SetImageServerView`

``SetImageServerView(modelCoord: `Datatype.CFrame`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.Camera:SetRoll`

``SetRoll(rollAngle: `float`)`` -> `null`

### `Class.Camera:TiltUnits`

``TiltUnits(units: `int`)`` -> `bool`
  [Deprecated]

### `Class.Camera:ViewportPointToRay`

``ViewportPointToRay(x: `float`, y: `float`, depth: `float`)`` -> `Datatype.Ray`

### `Class.Camera:WorldToScreenPoint`

``WorldToScreenPoint(worldPoint: `Datatype.Vector3`)`` -> `Tuple`

### `Class.Camera:WorldToViewportPoint`

``WorldToViewportPoint(worldPoint: `Datatype.Vector3`)`` -> `Tuple`

### `Class.Camera:Zoom`

``Zoom(distance: `float`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.Camera:ZoomToExtents`

``ZoomToExtents(boundingBoxCFrame: `Datatype.CFrame`, boundingBoxSize: `Datatype.Vector3`)`` -> `null`

## Events

### `Class.Camera.FirstPersonTransition`

Fires with: (entering: `bool`)

### `Class.Camera.InterpolationFinished`

Fires with: ()

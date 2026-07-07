---
title: Camera
type: class
superclass: PVInstance
tags: [NotReplicated]
---

# Camera

**Inherits from:** `Class.PVInstance` > `Class.Instance` > `Class.Object`

**Tags:** [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
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

``GetLargestCutoffDistance(ignoreList: `Datatype.Instances`)`` → `float`
  [Deprecated]

### `Class.Camera:GetPanSpeed`

``GetPanSpeed()`` → `float`
  [Deprecated]

### `Class.Camera:GetPartsObscuringTarget`

``GetPartsObscuringTarget(castPoints: `Array`, ignoreList: `Datatype.Instances`)`` → `Datatype.Instances`

### `Class.Camera:GetRenderCFrame`

``GetRenderCFrame()`` → `Datatype.CFrame`

### `Class.Camera:GetRoll`

``GetRoll()`` → `float`

### `Class.Camera:GetTiltSpeed`

``GetTiltSpeed()`` → `float`
  [Deprecated]

### `Class.Camera:Interpolate`

``Interpolate(endPos: `Datatype.CFrame`, endFocus: `Datatype.CFrame`, duration: `float`)`` → `null`
  [Deprecated]

### `Class.Camera:PanUnits`

``PanUnits(units: `int`)`` → `null`
  [Deprecated]

### `Class.Camera:ScreenPointToRay`

``ScreenPointToRay(x: `float`, y: `float`, depth: `float`)`` → `Datatype.Ray`

### `Class.Camera:SetCameraPanMode`

``SetCameraPanMode(mode: `Enum.CameraPanMode`)`` → `null`
  [Deprecated]

### `Class.Camera:SetImageServerView`

``SetImageServerView(modelCoord: `Datatype.CFrame`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Camera:SetRoll`

``SetRoll(rollAngle: `float`)`` → `null`

### `Class.Camera:TiltUnits`

``TiltUnits(units: `int`)`` → `bool`
  [Deprecated]

### `Class.Camera:ViewportPointToRay`

``ViewportPointToRay(x: `float`, y: `float`, depth: `float`)`` → `Datatype.Ray`

### `Class.Camera:WorldToScreenPoint`

``WorldToScreenPoint(worldPoint: `Datatype.Vector3`)`` → `Tuple`

### `Class.Camera:WorldToViewportPoint`

``WorldToViewportPoint(worldPoint: `Datatype.Vector3`)`` → `Tuple`

### `Class.Camera:Zoom`

``Zoom(distance: `float`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.Camera:ZoomToExtents`

``ZoomToExtents(boundingBoxCFrame: `Datatype.CFrame`, boundingBoxSize: `Datatype.Vector3`)`` → `null`

## Events

### `Class.Camera.FirstPersonTransition`

Fires with: (entering: `bool`)

### `Class.Camera.InterpolationFinished`

Fires with: ()

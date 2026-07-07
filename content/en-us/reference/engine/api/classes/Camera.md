---
title: Camera
type: class
superclass: PVInstance
tags: [NotReplicated]
---

# Camera

**Inherits**: PVInstance > Instance > Object

**Tags**: NotReplicated

## Properties

- **CFrame**: `CFrame`
- **CameraSubject**: `Instance`
- **CameraType**: `CameraType`
- **CoordinateFrame**: `CFrame` [Hidden] [NotReplicated] [Deprecated]
- **DiagonalFieldOfView**: `float` [NotReplicated]
- **FieldOfView**: `float`
- **FieldOfViewMode**: `FieldOfViewMode`
- **Focus**: `CFrame`
- **HeadLocked**: `bool`
- **HeadScale**: `float`
- **MaxAxisFieldOfView**: `float` [NotReplicated]
- **NearPlaneZ**: `float` [ReadOnly] [NotReplicated]
- **VRTiltAndRollEnabled**: `bool`
- **ViewportSize**: `Vector2` [ReadOnly] [NotReplicated]
- **focus**: `CFrame` [NotReplicated] [Deprecated]

## Methods

- **GetLargestCutoffDistance**(`ignoreList: Instances`) -> `float` [Deprecated]
- **GetPanSpeed**() -> `float` [Deprecated]
- **GetPartsObscuringTarget**(`castPoints: Array`, `ignoreList: Instances`) -> `Instances`
- **GetRenderCFrame**() -> `CFrame`
- **GetRoll**() -> `float`
- **GetTiltSpeed**() -> `float` [Deprecated]
- **Interpolate**(`endPos: CFrame`, `endFocus: CFrame`, `duration: float`) -> `null` [Deprecated]
- **PanUnits**(`units: int`) -> `null` [Deprecated]
- **ScreenPointToRay**(`x: float`, `y: float`, `depth: float = 0`) -> `Ray`
- **SetCameraPanMode**(`mode: CameraPanMode = Classic`) -> `null` [Deprecated]
- **SetImageServerView**(`modelCoord: CFrame`) -> `null`
- **SetRoll**(`rollAngle: float`) -> `null`
- **TiltUnits**(`units: int`) -> `bool` [Deprecated]
- **ViewportPointToRay**(`x: float`, `y: float`, `depth: float = 0`) -> `Ray`
- **WorldToScreenPoint**(`worldPoint: Vector3`) -> `Tuple`
- **WorldToViewportPoint**(`worldPoint: Vector3`) -> `Tuple`
- **Zoom**(`distance: float`) -> `bool`
- **ZoomToExtents**(`boundingBoxCFrame: CFrame`, `boundingBoxSize: Vector3`) -> `null`

## Events

- **FirstPersonTransition**(`entering: bool`)
- **InterpolationFinished**()

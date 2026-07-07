---
title: DragDetector
type: class
superclass: ClickDetector
---

# DragDetector

**Inherits**: ClickDetector > Instance > Object

## Properties

- **ActivatedCursorIcon**: `ContentId`
- **ActivatedCursorIconContent**: `Content`
- **ApplyAtCenterOfMass**: `bool`
- **Axis**: `Vector3` [NotReplicated]
- **DragFrame**: `CFrame`
- **DragStyle**: `DragDetectorDragStyle`
- **Enabled**: `bool`
- **GamepadModeSwitchKeyCode**: `KeyCode`
- **KeyboardModeSwitchKeyCode**: `KeyCode`
- **MaxDragAngle**: `float`
- **MaxDragTranslation**: `Vector3`
- **MaxForce**: `float`
- **MaxTorque**: `float`
- **MinDragAngle**: `float`
- **MinDragTranslation**: `Vector3`
- **Orientation**: `Vector3`
- **PermissionPolicy**: `DragDetectorPermissionPolicy`
- **ReferenceInstance**: `Instance`
- **ResponseStyle**: `DragDetectorResponseStyle`
- **Responsiveness**: `float`
- **RunLocally**: `bool`
- **SecondaryAxis**: `Vector3` [NotReplicated]
- **TrackballRadialPullFactor**: `float`
- **TrackballRollFactor**: `float`
- **VRSwitchKeyCode**: `KeyCode`
- **WorldAxis**: `Vector3` [NotReplicated]
- **WorldSecondaryAxis**: `Vector3` [NotReplicated]

## Methods

- **AddConstraintFunction**(`priority: int`, `function: Function`) -> `RBXScriptConnection`
- **GetReferenceFrame**() -> `CFrame`
- **RestartDrag**() -> `null`
- **SetDragStyleFunction**(`function: Function`) -> `null`
- **SetPermissionPolicyFunction**(`function: Function`) -> `null`

## Events

- **DragContinue**(`playerWhoDragged: Player`, `cursorRay: Ray`, `viewFrame: CFrame`, `vrInputFrame: OptionalCoordinateFrame`, `isModeSwitchKeyDown: bool`)
- **DragEnd**(`playerWhoDragged: Player`)
- **DragStart**(`playerWhoDragged: Player`, `cursorRay: Ray`, `viewFrame: CFrame`, `hitFrame: CFrame`, `clickedPart: BasePart`, `vrInputFrame: OptionalCoordinateFrame`, `isModeSwitchKeyDown: bool`)

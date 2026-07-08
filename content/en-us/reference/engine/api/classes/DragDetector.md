---
title: DragDetector
type: class
superclass: ClickDetector
---

# DragDetector

Instance which facilitates and encourages interaction with 3D objects in an
experience.

**Inherits from:** `Class.ClickDetector` > `Class.Instance` > `Class.Object`

## Description

The `Class.DragDetector` instance facilitates and encourages interaction with
3D objects in an experience, such as opening doors and drawers, sliding a part
around, and much more. Key features include:

- Place a `Class.DragDetector` under any `Class.BasePart` or `Class.Model` to
  make it draggable via all inputs (mouse, touch, gamepad, and VR), all
  without a single line of code.

- Choose from several `Class.DragDetector.DragStyle|DragStyle` options, define
  how the object responds to motion via
  `Class.DragDetector.ResponseStyle|ResponseStyle`, and optionally apply axis
  or movement limits.

- Scripts can respond to manipulation of dragged objects to drive UI or make
  logical decisions, such as adjusting the light level in a room based on a
  sliding wall switch dimmer.

- Players can manipulate anchored parts or models and they'll stay exactly
  where you put them upon release.

- `Class.DragDetector|DragDetectors` work in Studio as long as you're **not**
  using the **Select**, **Move**, **Scale**, or **Rotate** tools, making it
  easier to test and adjust draggable objects while editing.

See the [3D Drag Detectors](../../../ui/3D-drag-detectors.md) guide for
details and usage examples.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.DragDetector.ActivatedCursorIcon` | `Datatype.ContentId` |  |
| `Class.DragDetector.ActivatedCursorIconContent` | `Datatype.Content` |  |
| `Class.DragDetector.ApplyAtCenterOfMass` | `bool` |  |
| `Class.DragDetector.Axis` | `Datatype.Vector3` | [NotReplicated] |
| `Class.DragDetector.DragFrame` | `Datatype.CFrame` |  |
| `Class.DragDetector.DragStyle` | `Enum.DragDetectorDragStyle` |  |
| `Class.DragDetector.Enabled` | `bool` |  |
| `Class.DragDetector.GamepadModeSwitchKeyCode` | `Enum.KeyCode` |  |
| `Class.DragDetector.KeyboardModeSwitchKeyCode` | `Enum.KeyCode` |  |
| `Class.DragDetector.MaxDragAngle` | `float` |  |
| `Class.DragDetector.MaxDragTranslation` | `Datatype.Vector3` |  |
| `Class.DragDetector.MaxForce` | `float` |  |
| `Class.DragDetector.MaxTorque` | `float` |  |
| `Class.DragDetector.MinDragAngle` | `float` |  |
| `Class.DragDetector.MinDragTranslation` | `Datatype.Vector3` |  |
| `Class.DragDetector.Orientation` | `Datatype.Vector3` |  |
| `Class.DragDetector.PermissionPolicy` | `Enum.DragDetectorPermissionPolicy` |  |
| `Class.DragDetector.ReferenceInstance` | `Class.Instance` |  |
| `Class.DragDetector.ResponseStyle` | `Enum.DragDetectorResponseStyle` |  |
| `Class.DragDetector.Responsiveness` | `float` |  |
| `Class.DragDetector.RunLocally` | `bool` |  |
| `Class.DragDetector.SecondaryAxis` | `Datatype.Vector3` | [NotReplicated] |
| `Class.DragDetector.TrackballRadialPullFactor` | `float` |  |
| `Class.DragDetector.TrackballRollFactor` | `float` |  |
| `Class.DragDetector.VRSwitchKeyCode` | `Enum.KeyCode` |  |
| `Class.DragDetector.WorldAxis` | `Datatype.Vector3` | [NotReplicated] |
| `Class.DragDetector.WorldSecondaryAxis` | `Datatype.Vector3` | [NotReplicated] |

## Methods

### `Class.DragDetector:AddConstraintFunction`

``AddConstraintFunction(priority: `int`, function: `Datatype.Function`)`` -> `Datatype.RBXScriptConnection`

### `Class.DragDetector:GetReferenceFrame`

``GetReferenceFrame()`` -> `Datatype.CFrame`

### `Class.DragDetector:RestartDrag`

``RestartDrag()`` -> `null`

### `Class.DragDetector:SetDragStyleFunction`

``SetDragStyleFunction(function: `Datatype.Function`)`` -> `null`

### `Class.DragDetector:SetPermissionPolicyFunction`

``SetPermissionPolicyFunction(function: `Datatype.Function`)`` -> `null`

## Events

### `Class.DragDetector.DragContinue`

Fires with: (playerWhoDragged: `Class.Player`, cursorRay: `Datatype.Ray`, viewFrame: `Datatype.CFrame`, vrInputFrame: `Datatype.OptionalCoordinateFrame`, isModeSwitchKeyDown: `bool`)

### `Class.DragDetector.DragEnd`

Fires with: (playerWhoDragged: `Class.Player`)

### `Class.DragDetector.DragStart`

Fires with: (playerWhoDragged: `Class.Player`, cursorRay: `Datatype.Ray`, viewFrame: `Datatype.CFrame`, hitFrame: `Datatype.CFrame`, clickedPart: `Class.BasePart`, vrInputFrame: `Datatype.OptionalCoordinateFrame`, isModeSwitchKeyDown: `bool`)

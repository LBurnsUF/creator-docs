---
title: DragDetector
type: class
superclass: ClickDetector
---

# DragDetector

**Inherits from:** `Class.ClickDetector` > `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
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

``AddConstraintFunction(priority: `int`, function: `Datatype.Function`)`` → `Datatype.RBXScriptConnection`

### `Class.DragDetector:GetReferenceFrame`

``GetReferenceFrame()`` → `Datatype.CFrame`

### `Class.DragDetector:RestartDrag`

``RestartDrag()`` → `null`

### `Class.DragDetector:SetDragStyleFunction`

``SetDragStyleFunction(function: `Datatype.Function`)`` → `null`

### `Class.DragDetector:SetPermissionPolicyFunction`

``SetPermissionPolicyFunction(function: `Datatype.Function`)`` → `null`

## Events

### `Class.DragDetector.DragContinue`

Fires with: (playerWhoDragged: `Class.Player`, cursorRay: `Datatype.Ray`, viewFrame: `Datatype.CFrame`, vrInputFrame: `Datatype.OptionalCoordinateFrame`, isModeSwitchKeyDown: `bool`)

### `Class.DragDetector.DragEnd`

Fires with: (playerWhoDragged: `Class.Player`)

### `Class.DragDetector.DragStart`

Fires with: (playerWhoDragged: `Class.Player`, cursorRay: `Datatype.Ray`, viewFrame: `Datatype.CFrame`, hitFrame: `Datatype.CFrame`, clickedPart: `Class.BasePart`, vrInputFrame: `Datatype.OptionalCoordinateFrame`, isModeSwitchKeyDown: `bool`)

---
title: UIDragDetector
type: class
superclass: UIComponent
---

# UIDragDetector

**Inherits from:** `Class.UIComponent` > `Class.UIBase` > `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.UIDragDetector.ActivatedCursorIcon` | `Datatype.ContentId` |  |
| `Class.UIDragDetector.ActivatedCursorIconContent` | `Datatype.Content` |  |
| `Class.UIDragDetector.BoundingBehavior` | `Enum.UIDragDetectorBoundingBehavior` |  |
| `Class.UIDragDetector.BoundingUI` | `Class.GuiBase2d` |  |
| `Class.UIDragDetector.CursorIcon` | `Datatype.ContentId` |  |
| `Class.UIDragDetector.CursorIconContent` | `Datatype.Content` |  |
| `Class.UIDragDetector.DragAxis` | `Datatype.Vector2` |  |
| `Class.UIDragDetector.DragRelativity` | `Enum.UIDragDetectorDragRelativity` |  |
| `Class.UIDragDetector.DragRotation` | `float` |  |
| `Class.UIDragDetector.DragSpace` | `Enum.UIDragDetectorDragSpace` |  |
| `Class.UIDragDetector.DragStyle` | `Enum.UIDragDetectorDragStyle` |  |
| `Class.UIDragDetector.DragUDim2` | `Datatype.UDim2` |  |
| `Class.UIDragDetector.Enabled` | `bool` |  |
| `Class.UIDragDetector.MaxDragAngle` | `float` |  |
| `Class.UIDragDetector.MaxDragTranslation` | `Datatype.UDim2` |  |
| `Class.UIDragDetector.MinDragAngle` | `float` |  |
| `Class.UIDragDetector.MinDragTranslation` | `Datatype.UDim2` |  |
| `Class.UIDragDetector.ReferenceUIInstance` | `Class.GuiObject` |  |
| `Class.UIDragDetector.ResponseStyle` | `Enum.UIDragDetectorResponseStyle` |  |
| `Class.UIDragDetector.SelectionModeDragSpeed` | `Datatype.UDim2` |  |
| `Class.UIDragDetector.SelectionModeRotateSpeed` | `float` |  |
| `Class.UIDragDetector.UIDragSpeedAxisMapping` | `Enum.UIDragSpeedAxisMapping` |  |

## Methods

### `Class.UIDragDetector:AddConstraintFunction`

``AddConstraintFunction(priority: `int`, function: `Datatype.Function`)`` → `Datatype.RBXScriptConnection`

### `Class.UIDragDetector:GetReferencePosition`

``GetReferencePosition()`` → `Datatype.UDim2`

### `Class.UIDragDetector:GetReferenceRotation`

``GetReferenceRotation()`` → `float`

### `Class.UIDragDetector:SetDragStyleFunction`

``SetDragStyleFunction(function: `Datatype.Function`)`` → `null`

## Events

### `Class.UIDragDetector.DragContinue`

Fires with: (inputPosition: `Datatype.Vector2`)

### `Class.UIDragDetector.DragEnd`

Fires with: (inputPosition: `Datatype.Vector2`)

### `Class.UIDragDetector.DragStart`

Fires with: (inputPosition: `Datatype.Vector2`)

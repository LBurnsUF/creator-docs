---
title: UIDragDetector
type: class
superclass: UIComponent
---

# UIDragDetector

Instance which facilitates and encourages interaction with UI elements in an
experience.

**Inherits from:** `Class.UIComponent` > `Class.UIBase` > `Class.Instance` > `Class.Object`

## Description

The `Class.UIDragDetector` instance facilitates and encourages interaction
with 2D user interface elements in an experience, such as sliders and
spinners. Key features include:

- Place a `Class.UIDragDetector` under any `Class.GuiObject` instance to make
  it draggable via all inputs without a single line of code.

- Choose from several `Class.UIDragDetector.DragStyle|DragStyle` options,
  define how the object responds to motion via
  `Class.UIDragDetector.ResponseStyle|ResponseStyle`, and optionally apply
  axis, movement limits, or drag boundaries.

- Scripts can respond to manipulation of dragged objects to drive logic
  responses, such as adjusting settings.

- `Class.UIDragDetector|UIDragDetectors` work in Studio as long as you're
  **not** using the **Select**, **Move**, **Scale**, or **Rotate** tools, nor
  certain plugins or Studio's **UI** editor tools.

## Properties

| Property | Type | Description |
|----------|------|-------------|
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

``AddConstraintFunction(priority: `int`, function: `Datatype.Function`)`` -> `Datatype.RBXScriptConnection`

### `Class.UIDragDetector:GetReferencePosition`

``GetReferencePosition()`` -> `Datatype.UDim2`

### `Class.UIDragDetector:GetReferenceRotation`

``GetReferenceRotation()`` -> `float`

### `Class.UIDragDetector:SetDragStyleFunction`

``SetDragStyleFunction(function: `Datatype.Function`)`` -> `null`

## Events

### `Class.UIDragDetector.DragContinue`

Fires with: (inputPosition: `Datatype.Vector2`)

### `Class.UIDragDetector.DragEnd`

Fires with: (inputPosition: `Datatype.Vector2`)

### `Class.UIDragDetector.DragStart`

Fires with: (inputPosition: `Datatype.Vector2`)

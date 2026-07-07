---
title: UIDragDetector
type: class
superclass: UIComponent
---

# UIDragDetector

**Inherits**: UIComponent > UIBase > Instance > Object

## Properties

- **ActivatedCursorIcon**: `ContentId`
- **ActivatedCursorIconContent**: `Content`
- **BoundingBehavior**: `UIDragDetectorBoundingBehavior`
- **BoundingUI**: `GuiBase2d`
- **CursorIcon**: `ContentId`
- **CursorIconContent**: `Content`
- **DragAxis**: `Vector2`
- **DragRelativity**: `UIDragDetectorDragRelativity`
- **DragRotation**: `float`
- **DragSpace**: `UIDragDetectorDragSpace`
- **DragStyle**: `UIDragDetectorDragStyle`
- **DragUDim2**: `UDim2`
- **Enabled**: `bool`
- **MaxDragAngle**: `float`
- **MaxDragTranslation**: `UDim2`
- **MinDragAngle**: `float`
- **MinDragTranslation**: `UDim2`
- **ReferenceUIInstance**: `GuiObject`
- **ResponseStyle**: `UIDragDetectorResponseStyle`
- **SelectionModeDragSpeed**: `UDim2`
- **SelectionModeRotateSpeed**: `float`
- **UIDragSpeedAxisMapping**: `UIDragSpeedAxisMapping`

## Methods

- **AddConstraintFunction**(`priority: int`, `function: Function`) -> `RBXScriptConnection`
- **GetReferencePosition**() -> `UDim2`
- **GetReferenceRotation**() -> `float`
- **SetDragStyleFunction**(`function: Function`) -> `null`

## Events

- **DragContinue**(`inputPosition: Vector2`)
- **DragEnd**(`inputPosition: Vector2`)
- **DragStart**(`inputPosition: Vector2`)

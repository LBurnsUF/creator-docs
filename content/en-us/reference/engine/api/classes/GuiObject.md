---
title: GuiObject
type: class
superclass: GuiBase2d
tags: [NotCreatable, NotBrowsable]
---

# GuiObject

An abstract class for all 2D user interface objects.

**Inherits from:** `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotBrowsable]

## Description

`Class.GuiObject` is an abstract class (much like `Class.BasePart`) for a 2D
user interface object. It defines all the properties relating to the display
of a graphical user interface (GUI) object such as `Class.GuiObject.Size|Size`
and `Class.GuiObject.Position|Position`. It also has some useful read‑only
properties like `Class.GuiObject.AbsolutePosition|AbsolutePosition`,
`Class.GuiObject.AbsoluteSize|AbsoluteSize`, and
`Class.GuiObject.AbsoluteRotation|AbsoluteRotation`.

To manipulate the layout of GUI objects in special ways, you can use a layout
structure such as [list/flex](../../../ui/list-flex-layouts.md) or
[grid](../../../ui/grid-table-layouts.md), and you can style them beyond their
core properties through
[appearance modifiers](../../../ui/appearance-modifiers.md).

Although it's possible to detect mouse button events on any GUI object using
`Class.GuiObject.InputBegan|InputBegan` and
`Class.GuiObject.InputEnded|InputEnded`, only `Class.ImageButton` and
`Class.TextButton` have convenient dedicated events such as
`Class.TextButton.Activated|Activated` to detect click/press.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.GuiObject.Active` | `bool` |  |
| `Class.GuiObject.AnchorPoint` | `Datatype.Vector2` |  |
| `Class.GuiObject.AutomaticSize` | `Enum.AutomaticSize` |  |
| `Class.GuiObject.BackgroundColor` | `Datatype.BrickColor` | [Hidden] [NotReplicated] [Deprecated] |
| `Class.GuiObject.BackgroundColor3` | `Datatype.Color3` |  |
| `Class.GuiObject.BackgroundTransparency` | `float` |  |
| `Class.GuiObject.BorderColor` | `Datatype.BrickColor` | [Hidden] [NotReplicated] [Deprecated] |
| `Class.GuiObject.BorderColor3` | `Datatype.Color3` |  |
| `Class.GuiObject.BorderMode` | `Enum.BorderMode` |  |
| `Class.GuiObject.BorderSizePixel` | `int` |  |
| `Class.GuiObject.ClipsDescendants` | `bool` |  |
| `Class.GuiObject.Draggable` | `bool` | [Deprecated] |
| `Class.GuiObject.GuiState` | `Enum.GuiState` | [ReadOnly] [NotReplicated] |
| `Class.GuiObject.InputSink` | `Enum.InputSink` |  |
| `Class.GuiObject.Interactable` | `bool` |  |
| `Class.GuiObject.LayoutOrder` | `int` |  |
| `Class.GuiObject.NextSelectionDown` | `Class.GuiObject` |  |
| `Class.GuiObject.NextSelectionLeft` | `Class.GuiObject` |  |
| `Class.GuiObject.NextSelectionRight` | `Class.GuiObject` |  |
| `Class.GuiObject.NextSelectionUp` | `Class.GuiObject` |  |
| `Class.GuiObject.Position` | `Datatype.UDim2` |  |
| `Class.GuiObject.Rotation` | `float` |  |
| `Class.GuiObject.Selectable` | `bool` |  |
| `Class.GuiObject.SelectionImageObject` | `Class.GuiObject` |  |
| `Class.GuiObject.SelectionOrder` | `int` |  |
| `Class.GuiObject.SelectionRect2D` | `Datatype.Rect` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.GuiObject.Size` | `Datatype.UDim2` |  |
| `Class.GuiObject.SizeConstraint` | `Enum.SizeConstraint` |  |
| `Class.GuiObject.Transparency` | `float` | [Hidden] [NotReplicated] |
| `Class.GuiObject.Visible` | `bool` |  |
| `Class.GuiObject.ZIndex` | `int` |  |

## Methods

### `Class.GuiObject:TweenPosition`

``TweenPosition(endPosition: `Datatype.UDim2`, easingDirection: `Enum.EasingDirection`, easingStyle: `Enum.EasingStyle`, time: `float`, override: `bool`, callback: `Datatype.Function`)`` -> `bool`

### `Class.GuiObject:TweenPositionInternal`

``TweenPositionInternal(endPosition: `Datatype.UDim2`, easingDirection: `Enum.EasingDirection`, easingStyle: `Enum.EasingStyle`, time: `float`, override: `bool`, callback: `Datatype.Function`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.GuiObject:TweenSize`

``TweenSize(endSize: `Datatype.UDim2`, easingDirection: `Enum.EasingDirection`, easingStyle: `Enum.EasingStyle`, time: `float`, override: `bool`, callback: `Datatype.Function`)`` -> `bool`

### `Class.GuiObject:TweenSizeAndPosition`

``TweenSizeAndPosition(endSize: `Datatype.UDim2`, endPosition: `Datatype.UDim2`, easingDirection: `Enum.EasingDirection`, easingStyle: `Enum.EasingStyle`, time: `float`, override: `bool`, callback: `Datatype.Function`)`` -> `bool`

### `Class.GuiObject:TweenSizeAndPositionInternal`

``TweenSizeAndPositionInternal(endSize: `Datatype.UDim2`, endPosition: `Datatype.UDim2`, easingDirection: `Enum.EasingDirection`, easingStyle: `Enum.EasingStyle`, time: `float`, override: `bool`, callback: `Datatype.Function`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.GuiObject:TweenSizeInternal`

``TweenSizeInternal(endSize: `Datatype.UDim2`, easingDirection: `Enum.EasingDirection`, easingStyle: `Enum.EasingStyle`, time: `float`, override: `bool`, callback: `Datatype.Function`)`` -> `bool`
   {security: RobloxScriptSecurity}

## Events

### `Class.GuiObject.DragBegin`

Fires with: (initialPosition: `Datatype.UDim2`)
  [Deprecated]

### `Class.GuiObject.DragStopped`

Fires with: (x: `int`, y: `int`)
  [Deprecated]

### `Class.GuiObject.InputBegan`

Fires with: (input: `Class.InputObject`)

### `Class.GuiObject.InputChanged`

Fires with: (input: `Class.InputObject`)

### `Class.GuiObject.InputEnded`

Fires with: (input: `Class.InputObject`)

### `Class.GuiObject.MouseEnter`

Fires with: (x: `int`, y: `int`)

### `Class.GuiObject.MouseLeave`

Fires with: (x: `int`, y: `int`)

### `Class.GuiObject.MouseMoved`

Fires with: (x: `int`, y: `int`)

### `Class.GuiObject.MouseWheelBackward`

Fires with: (x: `int`, y: `int`)

### `Class.GuiObject.MouseWheelForward`

Fires with: (x: `int`, y: `int`)

### `Class.GuiObject.SelectionGained`

Fires with: ()

### `Class.GuiObject.SelectionLost`

Fires with: ()

### `Class.GuiObject.TouchLongPress`

Fires with: (touchPositions: `Array`, state: `Enum.UserInputState`)

### `Class.GuiObject.TouchPan`

Fires with: (touchPositions: `Array`, totalTranslation: `Datatype.Vector2`, velocity: `Datatype.Vector2`, state: `Enum.UserInputState`)

### `Class.GuiObject.TouchPinch`

Fires with: (touchPositions: `Array`, scale: `float`, velocity: `float`, state: `Enum.UserInputState`)

### `Class.GuiObject.TouchRotate`

Fires with: (touchPositions: `Array`, rotation: `float`, velocity: `float`, state: `Enum.UserInputState`)

### `Class.GuiObject.TouchSwipe`

Fires with: (swipeDirection: `Enum.SwipeDirection`, numberOfTouches: `int`)

### `Class.GuiObject.TouchTap`

Fires with: (touchPositions: `Array`)

---
title: GuiButton
type: class
superclass: GuiObject
tags: [NotCreatable, NotBrowsable]
---

# GuiButton

An abstract class for interactive 2D user interface elements.

**Inherits from:** `Class.GuiObject` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotBrowsable]

## Description

`Class.GuiButton` is an abstract class that inherits from `Class.GuiObject`.
It is the base class for the interactive, clickable `Class.ImageButton` and
`Class.TextButton` objects. This class also defines several properties for
interactive behavior, namely `Class.GuiButton.AutoButtonColor|AutoButtonColor`
and `Class.GuiButton.Modal|Modal`.

The most important event of a `Class.GuiButton` is
`Class.GuiButton.Activated|Activated`, a **multi-platform event** that fires
when the button is activated. When using a mouse, this means clicking the
button and releasing with the cursor still over the UI object. For touch, the
same applies but with a touch instead of button press. Finally, for gamepads,
`Class.GuiButton.Activated|Activated` fires if a `Class.GuiButton` is selected
when the **A** button is pressed and released. In short, this event is very
useful for multi-platform user interface programming as it provides a nice
general interface for a single user input.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.GuiButton.AutoButtonColor` | `bool` |  |
| `Class.GuiButton.HoverHapticEffect` | `Class.HapticEffect` |  |
| `Class.GuiButton.Modal` | `bool` |  |
| `Class.GuiButton.PressHapticEffect` | `Class.HapticEffect` |  |
| `Class.GuiButton.Selected` | `bool` |  |
| `Class.GuiButton.Style` | `Enum.ButtonStyle` |  |

## Events

### `Class.GuiButton.Activated`

Fires with: (inputObject: `Class.InputObject`, clickCount: `int`)

### `Class.GuiButton.MouseButton1Click`

Fires with: ()

### `Class.GuiButton.MouseButton1Down`

Fires with: (x: `int`, y: `int`)

### `Class.GuiButton.MouseButton1Up`

Fires with: (x: `int`, y: `int`)

### `Class.GuiButton.MouseButton2Click`

Fires with: ()

### `Class.GuiButton.MouseButton2Down`

Fires with: (x: `int`, y: `int`)

### `Class.GuiButton.MouseButton2Up`

Fires with: (x: `int`, y: `int`)

### `Class.GuiButton.SecondaryActivated`

Fires with: (inputObject: `Class.InputObject`)

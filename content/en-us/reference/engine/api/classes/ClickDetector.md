---
title: ClickDetector
type: class
superclass: Instance
---

# ClickDetector

An object that provides user input on in-experience `Class.BasePart|BaseParts`
and `Class.Model|Models`.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`ClickDetector` allows `Class.Script|Scripts` and
`Class.LocalScript|LocalScripts` to receive pointer input on 3D objects
through their `Class.ClickDetector.MouseClick|MouseClick` event. They work
when parented to `Class.BasePart`, `Class.Model`, or `Class.Folder` objects.
They detect basic mouse events: enter, leave, left click and right click.
Touch input on `Class.UserInputService.TouchEnabled|TouchEnabled` devices also
fires click events.

The default control scripts bind `Enum.KeyCode|ButtonR2` to interact with
`Class.ClickDetector|ClickDetectors` using
`Class.ContextActionService:BindActivate()`, which can also be used to
override this. When using gamepads, the center dot triggers
`Class.ClickDetector.MouseHoverEnter|MouseHoverEnter` and
`Class.ClickDetector.MouseHoverLeave|MouseHoverLeave`. The bound activation
button fires `Class.ClickDetector.MouseClick|MouseClick`.

`Class.ClickDetector.MaxActivationDistance|MaxActivationDistance` can be used
to limit the distance a player may be from a click detector before it is no
longer clickable.

`Class.ClickDetector` events fire on both the client and the server. Since a
`Class.LocalScript` will only run if it descends from a `Class.Player` or
player `Class.Player.Character|Character`, it's usually not useful to put a
`Class.LocalScript` inside a `Class.ClickDetector`, since the script won't run
or the object won't be clickable. If you need a `Class.LocalScript` to detect
`Class.ClickDetector` events, `Class.StarterPlayerScripts` may be a better
place instead.

#### Input Priority

If multiple `Class.ClickDetector|ClickDetectors` may detect user input, only
the deepest will fire events. If two `Class.ClickDetector|ClickDetectors` are
siblings, the first will take priority.

If an action bound with `Class.ContextActionService` uses the same input as a
`Class.ClickDetector`, the action bound with `Class.ContextActionService` will
take priority over the click detector's events.

`Class.UserInputService.InputBegan` will fire before `Class.ClickDetector`
events.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ClickDetector.CursorIcon` | `Datatype.ContentId` |  |
| `Class.ClickDetector.CursorIconContent` | `Datatype.Content` |  |
| `Class.ClickDetector.MaxActivationDistance` | `float` |  |

## Events

### `Class.ClickDetector.MouseClick`

Fires with: (playerWhoClicked: `Class.Player`)

### `Class.ClickDetector.MouseHoverEnter`

Fires with: (playerWhoHovered: `Class.Player`)

### `Class.ClickDetector.MouseHoverLeave`

Fires with: (playerWhoHovered: `Class.Player`)

### `Class.ClickDetector.RightMouseClick`

Fires with: (playerWhoClicked: `Class.Player`)

### `Class.ClickDetector.mouseClick`

Fires with: (playerWhoClicked: `Class.Player`)
  [Deprecated]

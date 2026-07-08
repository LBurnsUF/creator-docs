---
title: Handles
type: class
superclass: HandlesBase
---

# Handles

Places 3D handles around any object that its `Class.Handles.Adornee|Adornee`
is set to.

**Inherits from:** `Class.HandlesBase` > `Class.PartAdornment` > `Class.GuiBase3d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Description

The `Handles` object places 3D handles around any object that its
`Class.Handles.Adornee|Adornee` is set to; this property must be set to a 3D
object for the handles to appear. The color can be changed and the shape of
the handles can be set to either arrows or spheres.

For handles to be interactive, they must be parented to a player's
`Class.PlayerGui` or the `Class.CoreGui`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Handles.Faces` | `Datatype.Faces` |  |
| `Class.Handles.Style` | `Enum.HandlesStyle` |  |

## Events

### `Class.Handles.MouseButton1Down`

Fires with: (face: `Enum.NormalId`)

### `Class.Handles.MouseButton1Up`

Fires with: (face: `Enum.NormalId`)

### `Class.Handles.MouseDrag`

Fires with: (face: `Enum.NormalId`, distance: `float`)

### `Class.Handles.MouseEnter`

Fires with: (face: `Enum.NormalId`)

### `Class.Handles.MouseLeave`

Fires with: (face: `Enum.NormalId`)

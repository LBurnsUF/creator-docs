---
title: WireframeHandleAdornment
type: class
superclass: HandleAdornment
---

# WireframeHandleAdornment

Renders a wireframe adornment consisting of one or more lines onto a
`Class.BasePart` (including `Class.Terrain`) or into the `Class.Workspace`.

**Inherits from:** `Class.HandleAdornment` > `Class.PVAdornment` > `Class.GuiBase3d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Description

`WireframeHandleAdornment` renders a wireframe adornment consisting of one or
more lines onto a `Class.BasePart` (including `Class.Terrain`) or into the
`Class.Workspace`. If parented to a player's `Class.PlayerGui` or the
`Class.CoreGui`, this adornment can listen to input events for purposes such
as making dragger tools.

Note that a `WireframeHandleAdornment` instance **begins empty** and you must
add lines or paths to it through methods like
`Class.WireframeHandleAdornment:AddLines()|AddLines()` or
`Class.WireframeHandleAdornment:AddPath()|AddPath()`.

The rendered wireframe can be customized visually through its
`Class.WireframeHandleAdornment.Thickness|Thickness`,
`Class.WireframeHandleAdornment.Color3|Color3`, and
`Class.WireframeHandleAdornment.Transparency|Transparency` properties,
although these properties only affect subsequent draws and do not update lines
already drawn into the adornment.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.WireframeHandleAdornment.Scale` | `Datatype.Vector3` |  |
| `Class.WireframeHandleAdornment.Thickness` | `float` |  |

## Methods

### `Class.WireframeHandleAdornment:AddLine`

``AddLine(from: `Datatype.Vector3`, to: `Datatype.Vector3`)`` -> `null`

### `Class.WireframeHandleAdornment:AddLines`

``AddLines(points: `Array`)`` -> `null`

### `Class.WireframeHandleAdornment:AddPath`

``AddPath(points: `Array`, loop: `bool`)`` -> `null`

### `Class.WireframeHandleAdornment:AddText`

``AddText(point: `Datatype.Vector3`, text: `string`, size: `int`)`` -> `null`

### `Class.WireframeHandleAdornment:Clear`

``Clear()`` -> `null`

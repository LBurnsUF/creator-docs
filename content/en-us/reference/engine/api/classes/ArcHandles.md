---
title: ArcHandles
type: class
superclass: HandlesBase
---

# ArcHandles

The `Class.ArcHandles` object places 3D arc handles around any 3D object that
its `Class.PartAdornment.Adornee|Adornee` is set to.

**Inherits from:** `Class.HandlesBase` > `Class.PartAdornment` > `Class.GuiBase3d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Description

The **ArcHandles** object places 3D arc handles around any 3D object that its
`Class.PartAdornment.Adornee|Adornee` is set to. For handles to be
interactive, it must be parented to a player's `Class.PlayerGui` or the
`Class.CoreGui`.

<img src="../../../assets/engine-api/classes/ArcHandles/ArcHandles-Example.jpg"  alt="ArcHandles example" />

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ArcHandles.Axes` | `Datatype.Axes` |  |

## Events

### `Class.ArcHandles.MouseButton1Down`

Fires with: (axis: `Enum.Axis`)

### `Class.ArcHandles.MouseButton1Up`

Fires with: (axis: `Enum.Axis`)

### `Class.ArcHandles.MouseDrag`

Fires with: (axis: `Enum.Axis`, relativeAngle: `float`, deltaRadius: `float`)

### `Class.ArcHandles.MouseEnter`

Fires with: (axis: `Enum.Axis`)

### `Class.ArcHandles.MouseLeave`

Fires with: (axis: `Enum.Axis`)

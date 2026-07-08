---
title: HandleAdornment
type: class
superclass: PVAdornment
tags: [NotCreatable]
---

# HandleAdornment

An abstract class inherited by 3D handle adornments.

**Inherits from:** `Class.PVAdornment` > `Class.GuiBase3d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

`HandleAdornment` is an abstract class inherited by 3D handle adornments. If
parented to a player's `Class.PlayerGui` or the `Class.CoreGui`, handles can
listen to input events for purposes such as making dragger tools.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.HandleAdornment.AdornCullingMode` | `Enum.AdornCullingMode` |  |
| `Class.HandleAdornment.AlwaysOnTop` | `bool` |  |
| `Class.HandleAdornment.CFrame` | `Datatype.CFrame` |  |
| `Class.HandleAdornment.GizmoReference` | `Class.Instance` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.HandleAdornment.SizeRelativeOffset` | `Datatype.Vector3` |  |
| `Class.HandleAdornment.ZIndex` | `int` |  |

## Events

### `Class.HandleAdornment.MouseButton1Down`

Fires with: ()

### `Class.HandleAdornment.MouseButton1Up`

Fires with: ()

### `Class.HandleAdornment.MouseEnter`

Fires with: ()

### `Class.HandleAdornment.MouseLeave`

Fires with: ()

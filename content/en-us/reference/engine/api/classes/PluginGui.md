---
title: PluginGui
type: class
superclass: LayerCollector
tags: [NotCreatable, NotReplicated]
---

# PluginGui

**Inherits from:** `Class.LayerCollector` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.PluginGui.Plugin` | `Class.Plugin` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.PluginGui.Title` | `string` |  |

## Methods

### `Class.PluginGui:BindToClose`

``BindToClose(function: `Datatype.Function`)`` → `null`

### `Class.PluginGui:GetRelativeMousePosition`

``GetRelativeMousePosition()`` → `Datatype.Vector2`
   {security: PluginSecurity}

### `Class.PluginGui:OverrideStudioAction`

``OverrideStudioAction(studioAction: `Enum.StudioAction`)`` → `Class.StudioActionOverride`
   {security: RobloxScriptSecurity}

## Events

### `Class.PluginGui.InputBegan`

Fires with: (input: `Class.InputObject`, gameProcessedEvent: `bool`)

### `Class.PluginGui.InputChanged`

Fires with: (input: `Class.InputObject`, gameProcessedEvent: `bool`)

### `Class.PluginGui.InputEnded`

Fires with: (input: `Class.InputObject`, gameProcessedEvent: `bool`)

### `Class.PluginGui.MouseEnter`

Fires with: ()

### `Class.PluginGui.MouseLeave`

Fires with: ()

### `Class.PluginGui.PluginDragDropped`

Fires with: (dragData: `Dictionary`)

### `Class.PluginGui.PluginDragEntered`

Fires with: (dragData: `Dictionary`)

### `Class.PluginGui.PluginDragLeft`

Fires with: (dragData: `Dictionary`)

### `Class.PluginGui.PluginDragMoved`

Fires with: (dragData: `Dictionary`)

### `Class.PluginGui.PointerAction`

Fires with: (wheel: `float`, pan: `Datatype.Vector2`, pinch: `float`, gameProcessedEvent: `bool`)

### `Class.PluginGui.WindowFocusReleased`

Fires with: ()

### `Class.PluginGui.WindowFocused`

Fires with: ()

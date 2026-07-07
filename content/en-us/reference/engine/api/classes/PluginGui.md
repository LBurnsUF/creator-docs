---
title: PluginGui
type: class
superclass: LayerCollector
tags: [NotCreatable, NotReplicated]
---

# PluginGui

**Inherits**: LayerCollector > GuiBase2d > GuiBase > Instance > Object

**Tags**: NotCreatable, NotReplicated

## Properties

- **Plugin**: `Plugin` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Title**: `string`

## Methods

- **BindToClose**(`function: Function = nil`) -> `null`
- **GetRelativeMousePosition**() -> `Vector2`
- **OverrideStudioAction**(`studioAction: StudioAction`) -> `StudioActionOverride`

## Events

- **InputBegan**(`input: InputObject`, `gameProcessedEvent: bool`)
- **InputChanged**(`input: InputObject`, `gameProcessedEvent: bool`)
- **InputEnded**(`input: InputObject`, `gameProcessedEvent: bool`)
- **MouseEnter**()
- **MouseLeave**()
- **PluginDragDropped**(`dragData: Dictionary`)
- **PluginDragEntered**(`dragData: Dictionary`)
- **PluginDragLeft**(`dragData: Dictionary`)
- **PluginDragMoved**(`dragData: Dictionary`)
- **PointerAction**(`wheel: float`, `pan: Vector2`, `pinch: float`, `gameProcessedEvent: bool`)
- **WindowFocusReleased**()
- **WindowFocused**()

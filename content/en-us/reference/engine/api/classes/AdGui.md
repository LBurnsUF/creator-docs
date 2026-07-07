---
title: AdGui
type: class
superclass: SurfaceGuiBase
---

# AdGui

**Inherits**: SurfaceGuiBase > LayerCollector > GuiBase2d > GuiBase > Instance > Object

## Properties

- **AdShape**: `AdShape`
- **EnableVideoAds**: `bool`
- **FallbackImage**: `ContentId`
- **FallbackImageContent**: `Content`
- **Status**: `AdUnitStatus` [ReadOnly] [NotReplicated]

## Methods

- **GetSingleReportAdInfo**() -> `Map`
- **HandleLuaUIEvent**(`eventType: AdUIEventType`) -> `null`
- **forwardStateToLuaUI**() -> `null`

## Events

- **adGuiStateChanged**(`adUIState: Variant`)

## Callbacks

- **OnAdEvent**(`eventInfo: Dictionary`) -> `bool`

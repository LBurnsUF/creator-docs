---
title: AdGui
type: class
superclass: SurfaceGuiBase
---

# AdGui

**Inherits from:** `Class.SurfaceGuiBase` > `Class.LayerCollector` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.AdGui.AdShape` | `Enum.AdShape` |  |
| `Class.AdGui.EnableVideoAds` | `bool` |  |
| `Class.AdGui.FallbackImage` | `Datatype.ContentId` |  |
| `Class.AdGui.FallbackImageContent` | `Datatype.Content` |  |
| `Class.AdGui.Status` | `Enum.AdUnitStatus` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.AdGui:GetSingleReportAdInfo`

``GetSingleReportAdInfo()`` → `Map`
   {security: RobloxScriptSecurity}

### `Class.AdGui:HandleLuaUIEvent`

``HandleLuaUIEvent(eventType: `Enum.AdUIEventType`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AdGui:forwardStateToLuaUI`

``forwardStateToLuaUI()`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.AdGui.adGuiStateChanged`

Fires with: (adUIState: `Variant`)

## Callbacks

### `Class.AdGui.OnAdEvent`

``OnAdEvent(eventInfo: `Dictionary`)`` → `bool`

---
title: StarterGui
type: class
superclass: BasePlayerGui
tags: [NotCreatable, Service]
---

# StarterGui

**Inherits from:** `Class.BasePlayerGui` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.StarterGui.ClipsDescendantsSupportsRotation` | `Enum.RolloutState` | [NotScriptable] |
| `Class.StarterGui.ProcessUserInput` | `bool` | [Hidden] [NotReplicated] {security: PluginSecurity} |
| `Class.StarterGui.ResetPlayerGuiOnSpawn` | `bool` | [Deprecated] |
| `Class.StarterGui.RtlTextSupport` | `Enum.RtlTextSupport` | [NotScriptable] |
| `Class.StarterGui.ScreenOrientation` | `Enum.ScreenOrientation` |  |
| `Class.StarterGui.ShowDevelopmentGui` | `bool` |  |
| `Class.StarterGui.StudioDefaultStyleSheet` | `Class.StyleSheet` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.StarterGui.StudioInsertWidgetLayerCollectorAutoLinkStyleSheet` | `Class.StyleSheet` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.StarterGui.VirtualCursorMode` | `Enum.VirtualCursorMode` | [NotScriptable] |

## Methods

### `Class.StarterGui:GetCore`

``GetCore(parameterName: `string`)`` → `Variant`
  [Yields]

### `Class.StarterGui:GetCoreGuiEnabled`

``GetCoreGuiEnabled(coreGuiType: `Enum.CoreGuiType`)`` → `bool`

### `Class.StarterGui:RegisterGetCore`

``RegisterGetCore(parameterName: `string`, getFunction: `Datatype.Function`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.StarterGui:RegisterSetCore`

``RegisterSetCore(parameterName: `string`, setFunction: `Datatype.Function`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.StarterGui:SetCore`

``SetCore(parameterName: `string`, value: `Variant`)`` → `null`

### `Class.StarterGui:SetCoreGuiEnabled`

``SetCoreGuiEnabled(coreGuiType: `Enum.CoreGuiType`, enabled: `bool`)`` → `null`

## Events

### `Class.StarterGui.CoreGuiChangedSignal`

Fires with: (coreGuiType: `Enum.CoreGuiType`, enabled: `bool`)

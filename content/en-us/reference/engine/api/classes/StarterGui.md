---
title: StarterGui
type: class
superclass: BasePlayerGui
tags: [NotCreatable, Service]
---

# StarterGui

A container for `Class.LayerCollector` objects to be copied into the
`Class.PlayerGui` of `Class.Player|Players`. Also provides a range of
functions for interacting with the `Class.CoreGui`.

**Inherits from:** `Class.BasePlayerGui` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

`Class.StarterGui` is a container object designed to hold
`Class.LayerCollector` objects such as `Class.ScreenGui|ScreenGuis`.

When a `Class.Player.Character` spawns, the contents of their
`Class.PlayerGui` (if any) are emptied. Children of the `Class.StarterGui` are
then copied along with their descendants into the `Class.PlayerGui`. Note,
however, that `Class.LayerCollector` objects such as
`Class.ScreenGui|ScreenGuis` with their
`Class.LayerCollector.ResetOnSpawn|ResetOnSpawn` property set to `false` will
only be placed into each player's `Class.PlayerGui` once and will not be
deleted when the `Class.Player` respawns.

`Class.StarterGui` also includes a range of functions allowing you to interact
with the `Class.CoreGui`. For example `Class.StarterGui:SetCoreGuiEnabled()`
can be used to disable elements of the `Class.CoreGui`, and
`Class.StarterGui:SetCore()` can perform a range of functions including
creating notifications and system messages.

## Properties

| Property | Type | Description |
|----------|------|-------------|
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

``GetCore(parameterName: `string`)`` -> `Variant`
  [Yields]

### `Class.StarterGui:GetCoreGuiEnabled`

``GetCoreGuiEnabled(coreGuiType: `Enum.CoreGuiType`)`` -> `bool`

### `Class.StarterGui:RegisterGetCore`

``RegisterGetCore(parameterName: `string`, getFunction: `Datatype.Function`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StarterGui:RegisterSetCore`

``RegisterSetCore(parameterName: `string`, setFunction: `Datatype.Function`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StarterGui:SetCore`

``SetCore(parameterName: `string`, value: `Variant`)`` -> `null`

### `Class.StarterGui:SetCoreGuiEnabled`

``SetCoreGuiEnabled(coreGuiType: `Enum.CoreGuiType`, enabled: `bool`)`` -> `null`

## Events

### `Class.StarterGui.CoreGuiChangedSignal`

Fires with: (coreGuiType: `Enum.CoreGuiType`, enabled: `bool`)

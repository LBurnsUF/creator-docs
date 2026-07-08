---
title: Selection
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# Selection

The Selection service controls the `Class.Instance|Instances` that are
selected in Roblox Studio.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

The Selection service controls the `Class.Instance|Instances` that are
selected in Roblox Studio.

This service is particularly useful when developing `Class.Plugin|Plugins`, as
it allows the developer to access and manipulate the current selection.

Currently selected `Class.Instance|Instances` can be obtained and set using
the `Class.Selection:Get()` and `Class.Selection:Set()` functions. The
`Class.Selection.SelectionChanged` event fires whenever the current selection
changes.

For more information on using `Class.Selection` and `Class.Plugin|Plugins`,
see `Class.Plugin`.

Selection is also often used in the command bar, to set hidden properties or
run functions for selected `Class.Instance|Instances`.

Note this class only applies to Roblox Studio and has no applicability to
games.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Selection.ActiveInstance` | `Class.Instance` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Selection.RenderMode` | `Enum.SelectionRenderMode` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Selection.SelectionBoxThickness` | `float` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Selection.SelectionLineThickness` | `int` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Selection.SelectionThickness` | `float` | [ReadOnly] [NotReplicated] |
| `Class.Selection.ShowActiveInstanceHighlight` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |

## Methods

### `Class.Selection:Add`

``Add(instancesToAdd: `Datatype.Instances`)`` -> `null`
   {security: PluginSecurity}

### `Class.Selection:AddFocusCallback`

``AddFocusCallback(priority: `int`, function: `Datatype.Function`)`` -> `Datatype.RBXScriptConnection`
   {security: RobloxScriptSecurity}

### `Class.Selection:ClearTerrainSelectionHack`

``ClearTerrainSelectionHack()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.Selection:Get`

``Get()`` -> `Datatype.Instances`
   {security: PluginSecurity}

### `Class.Selection:Remove`

``Remove(instancesToRemove: `Datatype.Instances`)`` -> `null`
   {security: PluginSecurity}

### `Class.Selection:Set`

``Set(selection: `Datatype.Instances`)`` -> `null`
   {security: PluginSecurity}

### `Class.Selection:SetTerrainSelectionHack`

``SetTerrainSelectionHack(center: `Datatype.Vector3`, size: `Datatype.Vector3`)`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.Selection.SelectionChanged`

Fires with: ()

### `Class.Selection.SelectionChangedThisFrame`

Fires with: ()

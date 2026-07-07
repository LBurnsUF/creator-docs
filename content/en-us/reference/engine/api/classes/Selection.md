---
title: Selection
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# Selection

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.Selection.ActiveInstance` | `Class.Instance` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Selection.RenderMode` | `Enum.SelectionRenderMode` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Selection.SelectionBoxThickness` | `float` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Selection.SelectionLineThickness` | `int` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Selection.SelectionThickness` | `float` | [ReadOnly] [NotReplicated] |
| `Class.Selection.ShowActiveInstanceHighlight` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |

## Methods

### `Class.Selection:Add`

``Add(instancesToAdd: `Datatype.Instances`)`` → `null`
   {security: PluginSecurity}

### `Class.Selection:AddFocusCallback`

``AddFocusCallback(priority: `int`, function: `Datatype.Function`)`` → `Datatype.RBXScriptConnection`
   {security: RobloxScriptSecurity}

### `Class.Selection:ClearTerrainSelectionHack`

``ClearTerrainSelectionHack()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Selection:Get`

``Get()`` → `Datatype.Instances`
   {security: PluginSecurity}

### `Class.Selection:Remove`

``Remove(instancesToRemove: `Datatype.Instances`)`` → `null`
   {security: PluginSecurity}

### `Class.Selection:Set`

``Set(selection: `Datatype.Instances`)`` → `null`
   {security: PluginSecurity}

### `Class.Selection:SetTerrainSelectionHack`

``SetTerrainSelectionHack(center: `Datatype.Vector3`, size: `Datatype.Vector3`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.Selection.SelectionChanged`

Fires with: ()

### `Class.Selection.SelectionChangedThisFrame`

Fires with: ()

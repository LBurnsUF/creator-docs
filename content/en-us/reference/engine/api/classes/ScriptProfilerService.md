---
title: ScriptProfilerService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# ScriptProfilerService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.ScriptProfilerService:ClientRequestData`

``ClientRequestData(player: `Class.Player`)`` -> `null`
   {security: PluginSecurity}

### `Class.ScriptProfilerService:ClientStart`

``ClientStart(player: `Class.Player`, frequency: `int?`)`` -> `null`
   {security: PluginSecurity}

### `Class.ScriptProfilerService:ClientStop`

``ClientStop(player: `Class.Player`)`` -> `null`
   {security: PluginSecurity}

### `Class.ScriptProfilerService:DeserializeJSON`

``DeserializeJSON(jsonString: `string?`)`` -> `Dictionary`
  [CustomLuaState] {security: PluginSecurity}

### `Class.ScriptProfilerService:SaveScriptProfilingData`

``SaveScriptProfilingData(jsonString: `string`, filename: `string`)`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.ScriptProfilerService:ServerRequestData`

``ServerRequestData()`` -> `null`
   {security: PluginSecurity}

### `Class.ScriptProfilerService:ServerStart`

``ServerStart(frequency: `int?`)`` -> `null`
   {security: PluginSecurity}

### `Class.ScriptProfilerService:ServerStop`

``ServerStop()`` -> `null`
   {security: PluginSecurity}

## Events

### `Class.ScriptProfilerService.OnNewData`

Fires with: (player: `Class.Player`, jsonString: `string`)

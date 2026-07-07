---
title: ScriptProfilerService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# ScriptProfilerService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **ClientRequestData**(`player: Player`) -> `null`
- **ClientStart**(`player: Player`, `frequency: int?`) -> `null`
- **ClientStop**(`player: Player`) -> `null`
- **DeserializeJSON**(`jsonString: string?`) -> `Dictionary` [CustomLuaState]
- **SaveScriptProfilingData**(`jsonString: string`, `filename: string`) -> `string`
- **ServerRequestData**() -> `null`
- **ServerStart**(`frequency: int?`) -> `null`
- **ServerStop**() -> `null`

## Events

- **OnNewData**(`player: Player`, `jsonString: string`)

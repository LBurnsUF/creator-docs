---
title: ScriptDebuggerService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ScriptDebuggerService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **AddBreakpoint**(`scriptInstance: LuaSourceContainer`, `breakpoint: Dictionary`) -> `Dictionary`
- **ClearBreakpoints**() -> `null`
- **Evaluate**(`expression: string`, `frameId: int? = nil`) -> `Dictionary`
- **GetRootVariables**(`frameId: int`) -> `Array`
- **GetStackTrace**(`threadId: int`, `startFrame: int? = nil`) -> `Dictionary`
- **GetThreads**() -> `Array`
- **GetVariables**(`variablesReference: int`) -> `Array`
- **Pause**() -> `null`
- **RemoveBreakpoint**(`scriptInstance: LuaSourceContainer`, `line: int`) -> `bool`
- **SetExceptionBreakMode**(`breakMode: DebugBreakModeType`) -> `null`

## Events

- **Resumed**(`threadIds: Array`)

## Callbacks

- **OnStopped**(`stopped: Dictionary`) -> `Dictionary`

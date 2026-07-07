---
title: ScriptDebugger
type: class
superclass: Instance
tags: [NotCreatable]
---

# ScriptDebugger

**Inherits**: Instance > Object

**Tags**: NotCreatable

## Properties

- **CurrentLine**: `int` [ReadOnly] [NotReplicated]
- **IsDebugging**: `bool` [ReadOnly] [NotReplicated]
- **IsPaused**: `bool` [ReadOnly] [NotReplicated]
- **Script**: `Instance` [ReadOnly] [NotReplicated]

## Methods

- **AddWatch**(`expression: string`) -> `Instance`
- **GetBreakpoints**() -> `Instances`
- **GetGlobals**(`stackFrame: int = 0`) -> `Map`
- **GetLocals**(`stackFrame: int = 0`) -> `Map`
- **GetStack**() -> `Array`
- **GetUpvalues**(`stackFrame: int = 0`) -> `Map`
- **GetWatchValue**(`watch: Instance`) -> `Variant`
- **GetWatches**() -> `Instances`
- **SetBreakpoint**(`line: int`, `isContextDependentBreakpoint: bool`) -> `Instance`
- **SetGlobal**(`name: string`, `value: Variant`, `stackFrame: int`) -> `null`
- **SetLocal**(`name: string`, `value: Variant`, `stackFrame: int = 0`) -> `null`
- **SetUpvalue**(`name: string`, `value: Variant`, `stackFrame: int = 0`) -> `null`

## Events

- **BreakpointAdded**(`breakpoint: Instance`)
- **BreakpointRemoved**(`breakpoint: Instance`)
- **EncounteredBreak**(`line: int`, `breakReason: BreakReason`)
- **Resuming**()
- **WatchAdded**(`watch: Instance`)
- **WatchRemoved**(`watch: Instance`)

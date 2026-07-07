---
title: DebuggerManager
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# DebuggerManager

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **DebuggingEnabled**: `bool` [ReadOnly] [NotReplicated]

## Methods

- **AddDebugger**(`script: Instance`) -> `Instance`
- **EnableDebugging**() -> `null`
- **GetDebuggers**() -> `Instances`
- **Resume**() -> `null`
- **StepIn**() -> `null` [Deprecated]
- **StepOut**() -> `null` [Deprecated]
- **StepOver**() -> `null` [Deprecated]

## Events

- **DebuggerAdded**(`debugger: Instance`)
- **DebuggerRemoved**(`debugger: Instance`)

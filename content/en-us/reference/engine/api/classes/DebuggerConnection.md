---
title: DebuggerConnection
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# DebuggerConnection

**Inherits**: Instance > Object

**Tags**: NotCreatable, NotReplicated

## Properties

- **ErrorMessage**: `string` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **HasError**: `bool` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Id**: `int` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **IsPaused**: `bool` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **AddBreakpoint**(`script: string`, `line: int`, `breakpoint: Breakpoint`) -> `null`
- **Close**() -> `null`
- **EvaluateWatch**(`expression: string`, `frame: StackFrame`, `callback: Function`) -> `int`
- **GetFrameById**(`id: int`) -> `StackFrame`
- **GetSource**(`scriptRef: string`, `status: Function`) -> `int`
- **GetThreadById**(`id: int`) -> `ThreadState`
- **GetThreads**(`callback: Function`) -> `int`
- **GetVariableById**(`id: int`) -> `DebuggerVariable`
- **Pause**(`thread: ThreadState`, `status: Function`) -> `int`
- **Populate**(`instance: Instance`, `callback: Function`) -> `int`
- **RemoveBreakpoint**(`breakpoint: Breakpoint`) -> `null`
- **Resume**(`thread: ThreadState`, `status: Function`) -> `int`
- **SetExceptionBreakMode**(`breakMode: DebuggerExceptionBreakMode`, `callback: Function`) -> `int`
- **SetVariable**(`variable: DebuggerVariable`, `value: string`, `callback: Function`) -> `int`
- **Step**(`thread: ThreadState`, `callback: Function`) -> `int`
- **StepIn**(`thread: ThreadState`, `callback: Function`) -> `int`
- **StepOut**(`thread: ThreadState`, `callback: Function`) -> `int`
- **UpdateSelectedFrame**(`threadId: int`, `frameNumber: int`) -> `null`

## Events

- **BreakpointAdded**(`breakpoint: Breakpoint`)
- **BreakpointChanged**(`breakpoint: Breakpoint`)
- **BreakpointRemoved**(`breakpoint: Breakpoint`, `reason: BreakpointRemoveReason`)
- **Paused**(`pausedState: PausedState`, `reason: DebuggerPauseReason`)
- **Resumed**(`pausedState: PausedState`)

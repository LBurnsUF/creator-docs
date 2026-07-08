---
title: ScriptStoppedReason
type: enum
---

# `Enum.ScriptStoppedReason`

Describes why the debugger paused execution.

Passed in the `Datatype.ScriptDebugStopped` payload to the
`Class.ScriptDebuggerService.OnStopped` callback, indicating what triggered
the pause.

The `Enum.ScriptStoppedReason` enum has 5 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ScriptStoppedReason.Breakpoint` | 0 | Execution stopped because a user-defined breakpoint was hit. |
| `Enum.ScriptStoppedReason.Exception` | 1 | Execution stopped because an exception was thrown (governed by the current `Enum.DebugBreakModeType` |
| `Enum.ScriptStoppedReason.Pause` | 2 | Execution stopped because `Class.ScriptDebuggerService:Pause()` was called. |
| `Enum.ScriptStoppedReason.Step` | 3 | Execution stopped after completing a step operation. |
| `Enum.ScriptStoppedReason.Entry` | 4 | Execution stopped at a script's entry point. |

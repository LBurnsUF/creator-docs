---
title: DebuggerResumeType
type: enum
---

# `Enum.DebuggerResumeType`

Specifies how the debugger should resume execution after a pause.

Returned from the `Class.ScriptDebuggerService.OnStopped` callback (via
`Datatype.ScriptResumeAction`) to control how execution resumes after a
debugger pause.

The `Enum.DebuggerResumeType` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.DebuggerResumeType.StepInto` | 0 | Step into the next function call on the specified thread. |
| `Enum.DebuggerResumeType.StepOut` | 1 | Step out of the current function on the specified thread. |
| `Enum.DebuggerResumeType.StepOver` | 2 | Step over the current line on the specified thread. |
| `Enum.DebuggerResumeType.Resume` | 3 | Resume execution normally without stepping. |

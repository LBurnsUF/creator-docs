---
title: DebugBreakModeType
type: enum
---

# `Enum.DebugBreakModeType`

Controls when the debugger pauses on exceptions.

Used with `Class.ScriptDebuggerService:SetExceptionBreakMode()` to control
when the debugger pauses on exceptions. The mode applies to all
`Class.DataModel|DataModels`.

The `Enum.DebugBreakModeType` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.DebugBreakModeType.Never` | 0 | Never break on exceptions. |
| `Enum.DebugBreakModeType.Always` | 1 | Break on all exceptions. |
| `Enum.DebugBreakModeType.Unhandled` | 2 | Break only on unhandled exceptions. |

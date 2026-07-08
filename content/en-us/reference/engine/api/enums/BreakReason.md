---
title: BreakReason
type: enum
---

# `Enum.BreakReason`

Reason for the breakpoint hit.

Value for the reason the `Class.ScriptDebugger.EncounteredBreak` signal fired.

The `Enum.BreakReason` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.BreakReason.Other` | 0 | Pausing for a reason not covered by other values, for example if the user hit "Pause" button. |
| `Enum.BreakReason.Error` | 1 | Pausing on error hit in the code. |
| `Enum.BreakReason.SpecialBreakpoint` | 2 | Pausing on an internal breakpoint set by debugger command: e.g. step over, step into, step out of. |
| `Enum.BreakReason.UserBreakpoint` | 3 | Pausing on a user breakpoint. |

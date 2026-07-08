---
title: DebuggerPauseReason
type: enum
---

# `Enum.DebuggerPauseReason`

Reason that the DataModel was paused.

Reason that the DataModel was paused.

The `Enum.DebuggerPauseReason` enum has 6 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.DebuggerPauseReason.Unknown` | 0 | Pausing for a reason not covered by other values. |
| `Enum.DebuggerPauseReason.Requested` | 1 | Pause was requested by user. |
| `Enum.DebuggerPauseReason.Breakpoint` | 2 | Pausing on a user breakpoint. |
| `Enum.DebuggerPauseReason.Exception` | 3 | Pausing on error hit in the code. |
| `Enum.DebuggerPauseReason.SingleStep` | 4 | Pausing on an internal breakpoint set by debugger command: e.g. step over, step into, step out of. |
| `Enum.DebuggerPauseReason.Entrypoint` | 5 | Pausing at the entry on the script. |

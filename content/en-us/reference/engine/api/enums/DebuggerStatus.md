---
title: DebuggerStatus
type: enum
---

# `Enum.DebuggerStatus`

Result of a debugger request.

Result of a debugger request.

The `Enum.DebuggerStatus` enum has 9 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.DebuggerStatus.Success` | 0 | Request has completed successfully. |
| `Enum.DebuggerStatus.Timeout` | 1 | Timed out while waiting for response. |
| `Enum.DebuggerStatus.ConnectionLost` | 2 | Connection to the debugger was lost. |
| `Enum.DebuggerStatus.InvalidResponse` | 3 | Failed to parse response. |
| `Enum.DebuggerStatus.InternalError` | 4 | Exception encountered while processing response. |
| `Enum.DebuggerStatus.InvalidState` | 5 | The request was not appropriate for the current debugger state. |
| `Enum.DebuggerStatus.RpcError` | 6 | Response was an error. |
| `Enum.DebuggerStatus.InvalidArgument` | 7 | One of the request arguments was invalid. |
| `Enum.DebuggerStatus.ConnectionClosed` | 8 | Connection closed while waiting for response. |

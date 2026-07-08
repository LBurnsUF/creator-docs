---
title: DebuggerEndReason
type: enum
---

# `Enum.DebuggerEndReason`

Reason for the end of the debugger session.

Reason for the end of the debugger session.

The `Enum.DebuggerEndReason` enum has 8 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.DebuggerEndReason.ClientRequest` | 0 | Client requested connection termination. |
| `Enum.DebuggerEndReason.Timeout` | 1 | Connection timed out. |
| `Enum.DebuggerEndReason.InvalidHost` | 2 | Invalid host:port combination. |
| `Enum.DebuggerEndReason.Disconnected` | 3 | Connection was lost. |
| `Enum.DebuggerEndReason.ServerShutdown` | 4 | Server terminated the connection because it shut down. |
| `Enum.DebuggerEndReason.ServerProtocolMismatch` | 5 | Server has wrong version of protocol. |
| `Enum.DebuggerEndReason.ConfigurationFailed` | 6 | Got a failure response when trying to configure the server. |
| `Enum.DebuggerEndReason.RpcError` | 7 | An error occurred in the RPC layer. |

---
title: ReplicateInstanceDestroySetting
type: enum
---

# `Enum.ReplicateInstanceDestroySetting`

Controls how `Instance:Destroy()` calls are replicated from server to clients.

Determines the replication behavior the server uses when `Instance:Destroy()`
is called. This enum is used by
`Class.Workspace.ReplicateInstanceDestroySetting`.

The `Enum.ReplicateInstanceDestroySetting` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ReplicateInstanceDestroySetting.Default` | 0 | Uses the engine-default instance destroy replication behavior. |
| `Enum.ReplicateInstanceDestroySetting.Disabled` | 1 | Uses legacy instance destroy replication behavior. |
| `Enum.ReplicateInstanceDestroySetting.Enabled` | 2 | Uses improved instance destroy replication behavior. |

---
title: InstanceFileSyncStatus
type: enum
---

# `Enum.InstanceFileSyncStatus`

Describes the file sync status of an Instance.

Describes the file sync status of an `Class.Instance`.

The `Enum.InstanceFileSyncStatus` enum has 5 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.InstanceFileSyncStatus.NotSynced` | 0 | The `Class.Instance` is not being synced or errored. |
| `Enum.InstanceFileSyncStatus.Errored` | 1 | The `Class.Instance` is a sync root that has errored and stopped syncing. |
| `Enum.InstanceFileSyncStatus.SyncedAsRoot` | 2 | The `Class.Instance` is being synced as the root of a sync tree. |
| `Enum.InstanceFileSyncStatus.SyncedAsDescendant` | 3 | The `Class.Instance` is being synced because it is a descendant of a sync root. |
| `Enum.InstanceFileSyncStatus.AncestorErrored` | 4 | The `Class.Instance` is not currently being synced because the root of its sync tree is `Errored`. |

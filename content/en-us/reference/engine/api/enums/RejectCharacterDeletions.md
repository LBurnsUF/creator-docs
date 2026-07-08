---
title: RejectCharacterDeletions
type: enum
---

# `Enum.RejectCharacterDeletions`

Controls whether the server rejects client attempts to delete player
characters.

Determines whether the server rejects client replication requests that would
delete player character models from the workspace. This enum is used by
`Class.Workspace.RejectCharacterDeletions`.

The `Enum.RejectCharacterDeletions` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.RejectCharacterDeletions.Default` | 0 | Uses the engine-default behavior (currently equivalent to `Enabled`). |
| `Enum.RejectCharacterDeletions.Disabled` | 1 | The server does not reject character deletion requests from clients. |
| `Enum.RejectCharacterDeletions.Enabled` | 2 | The server rejects client attempts to delete player characters. |

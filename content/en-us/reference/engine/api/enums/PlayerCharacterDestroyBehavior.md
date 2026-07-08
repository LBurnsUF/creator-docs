---
title: PlayerCharacterDestroyBehavior
type: enum
---

# `Enum.PlayerCharacterDestroyBehavior`

Controls destruction behavior when a player character is removed.

Controls whether the engine automatically calls `Destroy()` on a player's old
character when it is replaced and on the `Player` object when the player
leaves. This enum is used by `Class.Workspace.PlayerCharacterDestroyBehavior`.

The `Enum.PlayerCharacterDestroyBehavior` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.PlayerCharacterDestroyBehavior.Default` | 0 | Uses the engine-default behavior. |
| `Enum.PlayerCharacterDestroyBehavior.Disabled` | 1 | Automatic `Destroy()` calls on character replacement and player removal are disabled. |
| `Enum.PlayerCharacterDestroyBehavior.Enabled` | 2 | The engine automatically calls `Destroy()` on old characters when they are replaced (for example, on |

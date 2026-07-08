---
title: LuauTypeCheckMode
type: enum
---

# `Enum.LuauTypeCheckMode`

The Luau type checking mode for scripts in the experience.

Determines how strictly the Luau type checker analyzes scripts in the
experience. This enum is used by `Class.Workspace.LuauTypeCheckMode`.

The `Enum.LuauTypeCheckMode` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.LuauTypeCheckMode.Default` | 0 | Uses the engine-default type checking mode. |
| `Enum.LuauTypeCheckMode.NoCheck` | 1 | Scripts are not type-checked. |
| `Enum.LuauTypeCheckMode.Nonstrict` | 2 | Scripts are type-checked in nonstrict mode. |
| `Enum.LuauTypeCheckMode.Strict` | 3 | Scripts are type-checked in strict mode. |

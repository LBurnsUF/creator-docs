---
title: AvatarUnificationMode
type: enum
---

# `Enum.AvatarUnificationMode`

Controls whether the R6 to R15 adapter is active, allowing R15 avatars to join
R6 experiences.

When enabled, R15 avatars joining an R6 experience receive adapter parts,
invisible `Class.MeshPart|MeshParts` with R6-compatible names welded to their
corresponding R15 parts. The adapter preserves R6-like scale and movement
while enabling R15 features such as layered clothing and animatable heads.
Used by `Class.Workspace.AvatarUnificationMode`.

The `Enum.AvatarUnificationMode` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.AvatarUnificationMode.Default` | 0 | Uses the engine-default avatar unification state. |
| `Enum.AvatarUnificationMode.Disabled` | 1 | Avatar unification is disabled. |
| `Enum.AvatarUnificationMode.Enabled` | 2 | Avatar unification is enabled. |

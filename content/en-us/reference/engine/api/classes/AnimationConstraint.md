---
title: AnimationConstraint
type: class
superclass: Constraint
---

# AnimationConstraint

Aligns two `Class.BasePart|BaseParts` with an animate-able kinematic or
force-based joint that supports physical simulation (ragdoll, arm strength).
The default joint type for R15 avatar rigs.

**Inherits from:** `Class.Constraint` > `Class.Instance` > `Class.Object`

## Description

#### Replaces Motor6D for Avatar rigs

As part of the
[Avatar Joint Upgrade](https://devforum.roblox.com/t/avatar-joint-upgrade-for-physically-simulated-character-movement-is-now-live/4298561),
`AnimationConstraint` is the **replacement for `Class.Motor6D`** in R15 player
character rigs. When
`Class.StarterPlayer.AvatarJointUpgrade|AvatarJointUpgrade` is enabled (the
default for new experiences), player characters spawn with
AnimationConstraints instead of Motor6Ds. Unlike Motor6D, AnimationConstraint
supports both kinematic animation and force-based physical simulation —
enabling ragdoll physics, arm strength, and other physically simulated
character movement without rebuilding the rig.

#### Migrating from Motor6D

If you have existing code that uses Motor6D for character rigs, note these key
differences. See also the
[Phase 2 migration recommendations](https://devforum.roblox.com/t/avatar-joint-upgrade-aju-phase-2-rollout-updated-migration-recommendations/4656414).

- **Finding joints**: Use `:FindFirstChildWhichIsA("AnimationConstraint")`
  instead of `:FindFirstChildOfClass("Motor6D")`. For code that must support
  both old and new rigs, check for AnimationConstraint first, then fall back
  to Motor6D.
- **C0, C1, Part0, Part1**: These properties exist on AnimationConstraint as
  **read-only** aliases for backwards compatibility. They map to
  `Attachment0.CFrame`, `Attachment1.CFrame`, `Attachment0.Parent`, and
  `Attachment1.Parent` respectively. Do not attempt to write to them.
- **Do not modify RigAttachment.CFrame directly** — this disrupts animation
  retargeting and causes performance issues.
- **Transform**: Works identically to `Class.Motor6D.Transform` — the
  `Class.Animator` writes to it each frame. Layer procedural animations by
  multiplying into `Transform` during `Class.RunService.PreSimulation`, which
  stacks with active animation tracks without breaking retargeting.
- **IsKinematic**: When `true` (default), behavior is equivalent to Motor6D.
  Set to `false` to enable force-based physical simulation.
- **Type checks**: `animConstraint:IsA("Motor6D")` returns `false`. Update any
  `IsA("Motor6D")` guards to also accept `"AnimationConstraint"`.
- **Server replication**: Instead of setting C0 on the server, use client-side
  animation evaluation and synchronize data through custom Attributes or
  `Class.UnreliableRemoteEvent`.

##### Example: Procedural neck rotation

```lua
-- Before (Motor6D): writing to C0 directly
local originalC0 = neck.C0
RunService.RenderStepped:Connect(function()
    neck.C0 = originalC0 * computeNeckRotation()
end)

-- After (AnimationConstraint): multiplying into Transform during PreSimulation
RunService.PreSimulation:Connect(function()
    if not animator.EvaluationThrottled then
        neck.Transform = computeNeckRotation() * neck.Transform
    end
end)
```

#### Description

An `AnimationConstraint` constrains its `Class.Attachment|Attachments` so that
they're offset by `Class.AnimationConstraint.Transform|Transform`. When
`Class.AnimationConstraint.IsKinematic|IsKinematic` is `true`, the parts
follow the transform perfectly (identical to Motor6D behavior). When `false`,
the constraint applies forces and torques limited by
`Class.AnimationConstraint.MaxForce|MaxForce` and
`Class.AnimationConstraint.MaxTorque|MaxTorque`, enabling physically simulated
character movement.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AnimationConstraint.AngularDamping` | `float` |  |
| `Class.AnimationConstraint.AngularStrength` | `float` |  |
| `Class.AnimationConstraint.C0` | `Datatype.CFrame` | [Hidden] [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.AnimationConstraint.C1` | `Datatype.CFrame` | [Hidden] [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.AnimationConstraint.EnableSkinning` | `bool` |  {security: RobloxScriptSecurity} |
| `Class.AnimationConstraint.IsKinematic` | `bool` |  |
| `Class.AnimationConstraint.LinearDamping` | `float` |  |
| `Class.AnimationConstraint.LinearStrength` | `float` |  |
| `Class.AnimationConstraint.MaxForce` | `float` |  |
| `Class.AnimationConstraint.MaxTorque` | `float` |  |
| `Class.AnimationConstraint.Part0` | `Class.BasePart` | [Hidden] [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.AnimationConstraint.Part1` | `Class.BasePart` | [Hidden] [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.AnimationConstraint.Transform` | `Datatype.CFrame` |  |

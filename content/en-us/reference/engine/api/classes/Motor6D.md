---
title: Motor6D
type: class
superclass: Motor
---

# Motor6D

Creates an animatable joint between two `Class.BasePart|BaseParts`. Superseded
by `Class.AnimationConstraint` for avatar/character rigs. Motor6D is no longer
used by default for player characters when
`Class.StarterPlayer.AvatarJointUpgrade|AvatarJointUpgrade` is enabled.

**Inherits from:** `Class.Motor` > `Class.JointInstance` > `Class.Instance` > `Class.Object`

## Description

#### Description

**Motor6D** joins two `Class.BasePart|BaseParts`
(`Class.JointInstance.Part0|Part0` and `Class.JointInstance.Part1|Part1`)
together in an animatable way. The `Class.Motor6D.Transform|Transform`
property determines the offset between these parts. This can be set manually
using `Class.RunService.PreSimulation` or through an `Class.Animator`.

Models whose parts are joined by `Class.Motor6D` are usually referred to as
**rigs**, typically for `Class.Humanoid|Humanoids`. Motor6D remains
appropriate for non-avatar mechanical rigs (doors, turrets, vehicles) where
physical simulation is not needed.

#### Transitioning to AnimationConstraint for Avatar rigs

As of the
[Avatar Joint Upgrade](https://devforum.roblox.com/t/avatar-joint-upgrade-for-physically-simulated-character-movement-is-now-live/4298561),
R15 player characters spawn with
`Class.AnimationConstraint|AnimationConstraints` instead of Motor6Ds when
`Class.StarterPlayer.AvatarJointUpgrade|AvatarJointUpgrade` is enabled (the
default for new experiences). Code that assumes character joints are Motor6Ds
— such as `character:FindFirstChildOfClass("Motor6D")` or
`joint:IsA("Motor6D")` — will not find joints on upgraded characters. Use
`Class.AnimationConstraint` for new avatar rig code. See the migration notes
on the `Class.AnimationConstraint` page.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Motor6D.ChildName` | `string` | [ReadOnly] [NotReplicated] [NotScriptable] |
| `Class.Motor6D.EnableSkinning` | `bool` |  {security: RobloxScriptSecurity} |
| `Class.Motor6D.ParentName` | `string` | [ReadOnly] [NotReplicated] [NotScriptable] |
| `Class.Motor6D.Transform` | `Datatype.CFrame` | [Hidden] [NotReplicated] |

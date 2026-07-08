---
title: AlignPosition
type: class
superclass: Constraint
---

# AlignPosition

Constraint which applies force to move two attachments together, or to move
one attachment to a goal position.

**Inherits from:** `Class.Constraint` > `Class.Instance` > `Class.Object`

## Description

The `AlignPosition` constraint applies force to move two attachments together,
or to move one attachment to a goal position. As indicated by the name, it
only affects the **position** of the attachments, not their orientation (to
align attachments by **orientation**, see `Class.AlignOrientation`).

When configuring this constraint, it may be helpful to study
[Roblox Units](../../../physics/units.md) to understand how Roblox units
compare to metric units.

#### Force Location

By default, force is applied to the parent of
`Class.Constraint.Attachment0|Attachment0` at that attachment's location,
meaning that if the parent's center of mass is not aligned with the direction
of the force, torque will be applied as well as force. Alternatively, force
can be applied to the parents' center of mass by toggling on
`Class.AlignPosition.ApplyAtCenterOfMass|ApplyAtCenterOfMass`.

#### Reactionary Force

By default, the constraint only applies force to
`Class.Constraint.Attachment0|Attachment0` while
`Class.Constraint.Attachment1|Attachment1` remains unaffected. If desired,
force can be applied to both attachments in **equal and opposite directions**
by enabling `Class.AlignPosition.ReactionForceEnabled|ReactionForceEnabled`.

#### Force Limits

You can configure this constraint to apply the maximum force that constraints
allow through the `Class.AlignPosition.RigidityEnabled|RigidityEnabled`
property. When `true`, the physics solver reacts as quickly as possible to
complete the alignment. When `false`, the force applied by the constraint is
limited based on `Class.AlignPosition.ForceLimitMode|ForceLimitMode`,
`Class.AlignPosition.MaxVelocity|MaxVelocity`, and
`Class.AlignPosition.Responsiveness|Responsiveness`. See
`Class.AlignPosition.ForceLimitMode|ForceLimitMode` for further details.

#### Attachment Mode

This constraint can use either **one** or **two** attachments in calculating
its goal. See `Class.AlignPosition.Mode|Mode` for details.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AlignPosition.ApplyAtCenterOfMass` | `bool` |  |
| `Class.AlignPosition.ForceLimitMode` | `Enum.ForceLimitMode` |  |
| `Class.AlignPosition.ForceRelativeTo` | `Enum.ActuatorRelativeTo` |  |
| `Class.AlignPosition.MaxAxesForce` | `Datatype.Vector3` |  |
| `Class.AlignPosition.MaxForce` | `float` |  |
| `Class.AlignPosition.MaxVelocity` | `float` |  |
| `Class.AlignPosition.Mode` | `Enum.PositionAlignmentMode` |  |
| `Class.AlignPosition.Position` | `Datatype.Vector3` |  |
| `Class.AlignPosition.ReactionForceEnabled` | `bool` |  |
| `Class.AlignPosition.Responsiveness` | `float` |  |
| `Class.AlignPosition.RigidityEnabled` | `bool` |  |

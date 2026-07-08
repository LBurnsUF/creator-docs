---
title: AlignOrientation
type: class
superclass: Constraint
---

# AlignOrientation

Constraint which applies torque to align two attachments, or to align one
attachment with a goal orientation.

**Inherits from:** `Class.Constraint` > `Class.Instance` > `Class.Object`

## Description

The `AlignOrientation` constraint applies torque to align two attachments, or
to align one attachment with a goal orientation. As indicated by the name, it
only affects the **orientation** of the attachments, not their position (to
align attachments **positionally**, see `Class.AlignPosition`).

Torque created by `AlignOrientation` is applied about the center of mass of
the parent of the attachments, or the center of mass of parts rigidly
connected to the parents.

When configuring this constraint, it may be helpful to study
[Roblox Units](../../../physics/units.md) to understand how Roblox units
compare to metric units.

#### Affected Axes

The axes affected by torque are controlled through the constraint's
`Class.AlignOrientation.AlignType|AlignType` property. When set to
`Enum.AlignType|PrimaryAxisParallel`,
`Enum.AlignType|PrimaryAxisPerpendicular` or
`Enum.AlignType|PrimaryAxisLookAt`, torque will only occur when the primary
axes become misaligned. Otherwise, the constraint will apply torque about all
3 axes to achieve alignment.

#### Reactionary Torque

By default, the constraint only applies torque to
`Class.Constraint.Attachment0|Attachment0` while
`Class.Constraint.Attachment1|Attachment1` remains unaffected. If desired,
torque can be applied to both attachments in **equal and opposite directions**
by enabling
`Class.AlignOrientation.ReactionTorqueEnabled|ReactionTorqueEnabled`.

#### Torque Magnitude

You can configure this constraint to apply the maximum torque that constraints
allow through the `Class.AlignOrientation.RigidityEnabled|RigidityEnabled`
property. When `true`, the physics solver reacts as quickly as possible to
complete the alignment. When `false`, the torque is determined by
`Class.AlignOrientation.MaxTorque|MaxTorque`,
`Class.AlignOrientation.MaxAngularVelocity|MaxAngularVelocity`, and
`Class.AlignOrientation.Responsiveness|Responsiveness`.

#### Attachment Mode

This constraint can use either **one** or **two** attachments in calculating
its goal. See `Class.AlignOrientation.Mode|Mode` for details.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AlignOrientation.AlignType` | `Enum.AlignType` |  |
| `Class.AlignOrientation.CFrame` | `Datatype.CFrame` |  |
| `Class.AlignOrientation.LookAtPosition` | `Datatype.Vector3` | [NotReplicated] |
| `Class.AlignOrientation.MaxAngularVelocity` | `float` |  |
| `Class.AlignOrientation.MaxTorque` | `float` |  |
| `Class.AlignOrientation.Mode` | `Enum.OrientationAlignmentMode` |  |
| `Class.AlignOrientation.PrimaryAxis` | `Datatype.Vector3` | [NotReplicated] |
| `Class.AlignOrientation.PrimaryAxisOnly` | `bool` |  |
| `Class.AlignOrientation.ReactionTorqueEnabled` | `bool` |  |
| `Class.AlignOrientation.Responsiveness` | `float` |  |
| `Class.AlignOrientation.RigidityEnabled` | `bool` |  |
| `Class.AlignOrientation.SecondaryAxis` | `Datatype.Vector3` | [NotReplicated] |

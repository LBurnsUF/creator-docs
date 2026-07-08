---
title: VectorForce
type: class
superclass: Constraint
---

# VectorForce

Applies constant force to an assembly.

**Inherits from:** `Class.Constraint` > `Class.Instance` > `Class.Object`

## Description

The `VectorForce` constraint applies constant force to an assembly. The
direction and strength of the force is determined by a `Datatype.Vector3` and
can be relative to an attachment on the part, another attachment, or the world
coordinate system. Alternatively:

- Because the `VectorForce` constraint applies **constant** force and
  acceleration, very high speeds may result if no other forces are involved.
  If you want to maintain a more steady velocity over time, use a
  `Class.LinearVelocity` constraint.
- If you only need **initial** velocity, set the
  `Class.BasePart.AssemblyLinearVelocity|AssemblyLinearVelocity` property
  directly on the assembly.

When configuring this constraint, it may be helpful to study
[Roblox Units](../../../physics/units.md) to understand how Roblox units
compare to metric units.

#### Force Location

By default, force is applied to the assembly at the location of
`Class.Constraint.Attachment0|Attachment0`. Thus, if its center of mass is not
aligned with the direction/point of force, torque will be applied as well. If
desired, force can be focused at the center of mass by toggling on
`Class.VectorForce.ApplyAtCenterOfMass|ApplyAtCenterOfMass`.

#### Relativity

By default, force is applied relative to
`Class.Constraint.Attachment0|Attachment0`. If the parent assembly rotates,
the force will change direction to match the adjusted orientation of the
attachment; visualize this behavior in how the thruster of a rocket pushes it
forward, regardless of the rocket's rotation.

If `Class.VectorForce.RelativeTo|RelativeTo` is set to
`Enum.ActuatorRelativeTo|World`, force will be applied in world coordinates,
independent of the parent or attachment orientations; visualize this behavior
as a directional force like the wind blowing against an object.

If `Class.VectorForce.RelativeTo|RelativeTo` is set to
`Enum.ActuatorRelativeTo|Attachment1`, force will be applied relative to
`Class.Constraint.Attachment1|Attachment1` and, if the attachment rotates, the
force will change to match its orientation.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.VectorForce.ApplyAtCenterOfMass` | `bool` |  |
| `Class.VectorForce.Force` | `Datatype.Vector3` |  |
| `Class.VectorForce.RelativeTo` | `Enum.ActuatorRelativeTo` |  |

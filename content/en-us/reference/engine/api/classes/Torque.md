---
title: Torque
type: class
superclass: Constraint
---

# Torque

Applies constant torque to an assembly from its center of mass.

**Inherits from:** `Class.Constraint` > `Class.Instance` > `Class.Object`

## Description

A `Torque` constraint applies constant torque to an assembly from its center
of mass. Alternatively:

- Because the `Torque` constraint applies **constant** torque and angular
  acceleration, very high speeds may result if no other forces are involved.
  If you want to maintain a more steady velocity over time, use an
  `Class.AngularVelocity` constraint.
- If you only need **initial** velocity, set the
  `Class.BasePart.AssemblyAngularVelocity|AssemblyAngularVelocity` property
  directly on the assembly.

When configuring this constraint, it may be helpful to study
[Roblox Units](../../../physics/units.md) to understand how Roblox units
compare to metric units.

#### Relativity

By default, torque is applied relative to
`Class.Constraint.Attachment0|Attachment0`. If the parent assembly rotates,
the torque will change direction to match the adjusted orientation of the
attachment.

If `Class.Torque.RelativeTo|RelativeTo` is set to
`Enum.ActuatorRelativeTo|World`, torque will be applied in world coordinates,
independent of the parent or attachment orientations.

If `Class.Torque.RelativeTo|RelativeTo` is set to
`Enum.ActuatorRelativeTo|Attachment1`, torque will be applied relative to
`Class.Constraint.Attachment1|Attachment1` and, if the attachment rotates,
change to match its orientation.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Torque.RelativeTo` | `Enum.ActuatorRelativeTo` |  |
| `Class.Torque.Torque` | `Datatype.Vector3` |  |

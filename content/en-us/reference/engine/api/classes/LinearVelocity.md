---
title: LinearVelocity
type: class
superclass: Constraint
---

# LinearVelocity

Applies force on an assembly to maintain a constant linear velocity.

**Inherits from:** `Class.Constraint` > `Class.Instance` > `Class.Object`

## Description

The `LinearVelocity` constraint applies force on an assembly to maintain a
**constant** linear velocity. It can be set to apply force along a
`Datatype.Vector3`, line, or 2D&nbsp;plane. Alternatively:

- If you want to control the amount of force applied, use a
  `Class.VectorForce` constraint.
- If you only need **initial** linear velocity, set the
  `Class.BasePart.AssemblyLinearVelocity|AssemblyLinearVelocity` property
  directly on the assembly.

When configuring this constraint, it may be helpful to study
[Roblox Units](../../../physics/units.md) to understand how Roblox units
compare to metric units.

#### Relativity

Application of velocity can be controlled through the constraint's
`Class.LinearVelocity.RelativeTo|RelativeTo` property. If set to
`Enum.ActuatorRelativeTo|World`, force will be applied in world coordinates,
independent of the parent or attachment orientations. If set to
`Enum.ActuatorRelativeTo|Attachment0` or
`Enum.ActuatorRelativeTo|Attachment1`, force will be applied relative to
`Class.Constraint.Attachment0|Attachment0` or
`Class.Constraint.Attachment1|Attachment1` respectively.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.LinearVelocity.ForceLimitMode` | `Enum.ForceLimitMode` |  |
| `Class.LinearVelocity.ForceLimitsEnabled` | `bool` |  |
| `Class.LinearVelocity.LineDirection` | `Datatype.Vector3` |  |
| `Class.LinearVelocity.LineVelocity` | `float` |  |
| `Class.LinearVelocity.MaxAxesForce` | `Datatype.Vector3` |  |
| `Class.LinearVelocity.MaxForce` | `float` |  |
| `Class.LinearVelocity.MaxPlanarAxesForce` | `Datatype.Vector2` |  |
| `Class.LinearVelocity.PlaneVelocity` | `Datatype.Vector2` |  |
| `Class.LinearVelocity.PrimaryTangentAxis` | `Datatype.Vector3` |  |
| `Class.LinearVelocity.ReactionForceEnabled` | `bool` |  |
| `Class.LinearVelocity.RelativeTo` | `Enum.ActuatorRelativeTo` |  |
| `Class.LinearVelocity.SecondaryTangentAxis` | `Datatype.Vector3` |  |
| `Class.LinearVelocity.VectorVelocity` | `Datatype.Vector3` |  |
| `Class.LinearVelocity.VelocityConstraintMode` | `Enum.VelocityConstraintMode` |  |

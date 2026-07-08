---
title: TorsionSpringConstraint
type: class
superclass: Constraint
---

# TorsionSpringConstraint

A rotational spring that opposes the angular motion between two axes.

**Inherits from:** `Class.Constraint` > `Class.Instance` > `Class.Object`

## Description

A **TorsionSpringConstraint** applies a torque based on a relative angle and a
relative angular velocity. Specifically, torsion springs try to bring two axes
from two parts together in a compliant way.

Correct orientation of a torsion spring's attachments is important. The
constraint will attempt to bring the
`Class.Attachment.SecondaryAxis|SecondaryAxis` of each attachment into
alignment. When building mechanisms like swinging doors, ensure that the
secondary axes are **perpendicular** to the intended axis of rotation.

When configuring this constraint, it may be helpful to study
[Roblox Units](../../../physics/units.md) to understand how Roblox units
compare to metric units.

#### Damping

The `Class.TorsionSpringConstraint.Damping|Damping` value controls how fast
the spring's oscillation dies down. A value of 0 allows the spring to
oscillate endlessly, while higher values bring the spring to a rest more
quickly.

#### Stiffness

`Class.TorsionSpringConstraint.Stiffness|Stiffness` sets the torsional
strength of the spring. Higher values create a spring that responds with more
force.

#### Limits

Enabling the `Class.TorsionSpringConstraint.LimitsEnabled|LimitsEnabled`
property exposes the `Class.TorsionSpringConstraint.MaxAngle|MaxAngle` value
to restrict the spring's range within a cone; it also exposes the
`Class.TorsionSpringConstraint.Restitution|Restitution` value which defines
the elasticity of the attachments when they reach their limit.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.TorsionSpringConstraint.Coils` | `float` |  |
| `Class.TorsionSpringConstraint.CurrentAngle` | `float` | [ReadOnly] [NotReplicated] |
| `Class.TorsionSpringConstraint.Damping` | `float` |  |
| `Class.TorsionSpringConstraint.LimitEnabled` | `bool` | [Hidden] [Deprecated] |
| `Class.TorsionSpringConstraint.LimitsEnabled` | `bool` |  |
| `Class.TorsionSpringConstraint.MaxAngle` | `float` |  |
| `Class.TorsionSpringConstraint.MaxTorque` | `float` |  |
| `Class.TorsionSpringConstraint.Radius` | `float` |  |
| `Class.TorsionSpringConstraint.Restitution` | `float` |  |
| `Class.TorsionSpringConstraint.Stiffness` | `float` |  |

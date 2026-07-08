---
title: SlidingBallConstraint
type: class
superclass: Constraint
tags: [NotCreatable]
---

# SlidingBallConstraint

The base class for constraints that allow their attachments to slide along an
axis but not rotate.

**Inherits from:** `Class.Constraint` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

**SlidingBallConstraint** is the base class for constraints that allow their
attachments to slide along an axis but not rotate, including
`Class.PrismaticConstraint` and `Class.CylindricalConstraint`. This constrains
the attachments so that their **X** axes are collinear but pointing in
opposite directions. It also constrains the attachments so that their **Y**
axes are parallel.

When configuring this constraint, it may be helpful to study
[Roblox Units](../../../physics/units.md) to understand how Roblox units
compare to metric units.

#### Linear Power

If this constraint's `Class.SlidingBallConstraint|ActuatorType` is set to
`Enum.ActuatorType|Motor`, it attempts to translate the attachments with the
goal of reaching `Class.SlidingBallConstraint|Velocity`. You can further
control this translation through both
`Class.SlidingBallConstraint|MotorMaxAcceleration` and
`Class.SlidingBallConstraint|MotorMaxForce`.

If this constraint's `Class.SlidingBallConstraint|ActuatorType` is set to
`Enum.ActuatorType|Servo`, it attempts to translate the attachments to a set
separation specified by `Class.SlidingBallConstraint|TargetPosition`. This
translation is controlled by `Class.SlidingBallConstraint|Speed`,
`Class.SlidingBallConstraint|LinearResponsiveness`, and
`Class.SlidingBallConstraint|ServoMaxForce`.

#### Limits

You can set **limits** to restrict this constraint's sliding range. Enabling
the `Class.SlidingBallConstraint|LimitsEnabled` property exposes the
`Class.SlidingBallConstraint|LowerLimit` and
`Class.SlidingBallConstraint|UpperLimit` values, as well as
`Class.SlidingBallConstraint|Restitution` which defines the elasticity of the
attachments when they reach either limit.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.SlidingBallConstraint.ActuatorType` | `Enum.ActuatorType` |  |
| `Class.SlidingBallConstraint.CurrentPosition` | `float` | [ReadOnly] [NotReplicated] |
| `Class.SlidingBallConstraint.LimitsEnabled` | `bool` |  |
| `Class.SlidingBallConstraint.LinearResponsiveness` | `float` |  |
| `Class.SlidingBallConstraint.LowerLimit` | `float` |  |
| `Class.SlidingBallConstraint.MotorMaxAcceleration` | `float` |  |
| `Class.SlidingBallConstraint.MotorMaxForce` | `float` |  |
| `Class.SlidingBallConstraint.Restitution` | `float` |  |
| `Class.SlidingBallConstraint.ServoMaxForce` | `float` |  |
| `Class.SlidingBallConstraint.Size` | `float` |  |
| `Class.SlidingBallConstraint.SoftlockServoUponReachingTarget` | `bool` | [Deprecated] |
| `Class.SlidingBallConstraint.Speed` | `float` |  |
| `Class.SlidingBallConstraint.TargetPosition` | `float` |  |
| `Class.SlidingBallConstraint.UpperLimit` | `float` |  |
| `Class.SlidingBallConstraint.Velocity` | `float` |  |

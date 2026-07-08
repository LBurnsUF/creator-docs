---
title: HingeConstraint
type: class
superclass: Constraint
---

# HingeConstraint

Constrains its attachments to rotate about a single axis.

**Inherits from:** `Class.Constraint` > `Class.Instance` > `Class.Object`

## Description

A **HingeConstraint** allows two `Class.Attachment|Attachments` to rotate
about one axis, constraining the two `Class.Attachment|Attachments` so that
they both occupy the same position and that their **X** axes point in the same
direction.

Note that if this constraint attaches one part (**A**) to another part (**B**)
that is anchored or connected to an anchored part (**Z**), part **A** will not
be locally simulated when interacting with a player.

When configuring this constraint, it may be helpful to study
[Roblox Units](../../../physics/units.md) to understand how Roblox units
compare to metric units.

#### Angular Power

Hinges can be configured to actuate rotation. If a hinge's
`Class.HingeConstraint.ActuatorType|ActuatorType` is set to
`Enum.ActuatorType|Motor`, it attempts to rotate the attachments with the goal
of reaching its `Class.HingeConstraint.AngularVelocity|AngularVelocity`. You
can further control this rotation through both
`Class.HingeConstraint.MotorMaxAcceleration|MotorMaxAcceleration` and
`Class.HingeConstraint.MotorMaxTorque|MotorMaxTorque`. If a hinge's
`Class.HingeConstraint.ActuatorType|ActuatorType` is set to
`Enum.ActuatorType|Servo`, it attempts to rotate to an angle specified by
`Class.HingeConstraint.TargetAngle|TargetAngle`. This rotation is controlled
by both `Class.HingeConstraint.AngularSpeed|AngularSpeed` and
`Class.HingeConstraint.ServoMaxTorque|ServoMaxTorque`.

#### Limits

You can set limits to restrict the rotation of a hinge, useful for mechanisms
like doors which should only swing open or closed within a set range. Enabling
the `Class.HingeConstraint.LimitsEnabled|LimitsEnabled` property exposes the
`Class.HingeConstraint.LowerAngle|LowerAngle` and
`Class.HingeConstraint.UpperAngle|UpperAngle` limits, as well as
`Class.HingeConstraint.Restitution|Restitution` which defines the elasticity
of the attachments when they reach either limit.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.HingeConstraint.ActuatorType` | `Enum.ActuatorType` |  |
| `Class.HingeConstraint.AngularResponsiveness` | `float` |  |
| `Class.HingeConstraint.AngularSpeed` | `float` |  |
| `Class.HingeConstraint.AngularVelocity` | `float` |  |
| `Class.HingeConstraint.CurrentAngle` | `float` | [ReadOnly] [NotReplicated] |
| `Class.HingeConstraint.LimitsEnabled` | `bool` |  |
| `Class.HingeConstraint.LowerAngle` | `float` |  |
| `Class.HingeConstraint.MotorMaxAcceleration` | `float` |  |
| `Class.HingeConstraint.MotorMaxTorque` | `float` |  |
| `Class.HingeConstraint.Radius` | `float` |  |
| `Class.HingeConstraint.Restitution` | `float` |  |
| `Class.HingeConstraint.ServoMaxTorque` | `float` |  |
| `Class.HingeConstraint.SoftlockServoUponReachingTarget` | `bool` | [Deprecated] |
| `Class.HingeConstraint.TargetAngle` | `float` |  |
| `Class.HingeConstraint.UpperAngle` | `float` |  |

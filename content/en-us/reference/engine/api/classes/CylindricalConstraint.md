---
title: CylindricalConstraint
type: class
superclass: SlidingBallConstraint
---

# CylindricalConstraint

Constrains two attachments on two parts to have a relative linear and
rotational motion.

**Inherits from:** `Class.SlidingBallConstraint` > `Class.Constraint` > `Class.Instance` > `Class.Object`

## Description

A **CylindricalConstraint** allows its attachments to slide along one axis and
rotate about another axis. It can be thought of like a combination of a
`Class.PrismaticConstraint` and a `Class.HingeConstraint`. The sliding axis is
determined by the **X** axis of the constraint's
`Class.Constraint.Attachment0|Attachment0`. The rotation axis is centered at
the constraint's `Class.Constraint.Attachment1|Attachment1` and is angled off
of the sliding constraint by the constraint's
`Class.CylindricalConstraint.InclinationAngle|InclinationAngle`.

This constraint, along with a `Class.SpringConstraint`, is ideal for building
vehicle suspension.

Note that if this constraint attaches one part (**A**) to another part (**B**)
that is anchored or connected to an anchored part (**Z**), part **A** will not
be locally simulated when interacting with a player.

When configuring this constraint, it may be helpful to study
[Roblox Units](../../../physics/units.md) to understand how Roblox units
compare to metric units.

#### Angular Power

If a cylindrical's
`Class.CylindricalConstraint.AngularActuatorType|AngularActuatorType` is set
to `Enum.ActuatorType|Motor`, it attempts to rotate the attachments with the
goal of reaching its
`Class.CylindricalConstraint.AngularVelocity|AngularVelocity`. You can further
control this rotation through both
`Class.CylindricalConstraint.MotorMaxAngularAcceleration|MotorMaxAngularAcceleration`
and `Class.CylindricalConstraint.MotorMaxTorque|MotorMaxTorque`. If a
cylindrical's
`Class.CylindricalConstraint.AngularActuatorType|AngularActuatorType` is set
to `Enum.ActuatorType|Servo`, it attempts to rotate to an angle specified by
`Class.CylindricalConstraint.TargetAngle|TargetAngle`. This rotation is
controlled by `Class.CylindricalConstraint.AngularSpeed|AngularSpeed`,
`Class.CylindricalConstraint.AngularResponsiveness|AngularResponsiveness`, and
`Class.CylindricalConstraint.ServoMaxTorque|ServoMaxTorque`.

#### Linear Power

If a cylindrical's `Class.CylindricalConstraint|ActuatorType` is set to
`Enum.ActuatorType|Motor`, it attempts to translate the attachments with the
goal of reaching `Class.CylindricalConstraint|Velocity`. You can further
control this translation through both
`Class.CylindricalConstraint|MotorMaxAcceleration` and
`Class.CylindricalConstraint|MotorMaxForce`. If a cylindrical's
`Class.CylindricalConstraint|ActuatorType` is set to
`Enum.ActuatorType|Servo`, it attempts to translate the attachments to a set
separation specified by `Class.CylindricalConstraint|TargetPosition`. This
translation is controlled by `Class.CylindricalConstraint|Speed`,
`Class.CylindricalConstraint|LinearResponsiveness`, and
`Class.CylindricalConstraint|ServoMaxForce`.

#### Limits

You can set limits to restrict both the **sliding range** and **rotation** of
a cylindrical constraint. Enabling the
`Class.CylindricalConstraint|LimitsEnabled` property exposes the
`Class.CylindricalConstraint|LowerLimit` and
`Class.CylindricalConstraint|UpperLimit` values, as well as
`Class.CylindricalConstraint|Restitution` which defines the elasticity of the
attachments when they reach either limit. Enabling the
`Class.CylindricalConstraint.AngularLimitsEnabled|AngularLimitsEnabled`
property exposes the `Class.CylindricalConstraint.LowerAngle|LowerAngle` and
`Class.CylindricalConstraint.UpperAngle|UpperAngle` limits, as well as
`Class.CylindricalConstraint.AngularRestitution|AngularRestitution` which
defines the elasticity of the attachments when they reach either limit.

#### Inclination Angle

`Class.CylindricalConstraint.InclinationAngle|InclinationAngle` defines the
direction of the rotation axis as an angle from the **X** axis in the **XY**
plane of `Class.Constraint.Attachment0|Attachment0`, from
-180&nbsp;to&nbsp;180. This lets you tilt the rotating element without
changing the sliding axis.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.CylindricalConstraint.AngularActuatorType` | `Enum.ActuatorType` |  |
| `Class.CylindricalConstraint.AngularLimitsEnabled` | `bool` |  |
| `Class.CylindricalConstraint.AngularResponsiveness` | `float` |  |
| `Class.CylindricalConstraint.AngularRestitution` | `float` |  |
| `Class.CylindricalConstraint.AngularSpeed` | `float` |  |
| `Class.CylindricalConstraint.AngularVelocity` | `float` |  |
| `Class.CylindricalConstraint.CurrentAngle` | `float` | [ReadOnly] [NotReplicated] |
| `Class.CylindricalConstraint.InclinationAngle` | `float` |  |
| `Class.CylindricalConstraint.LowerAngle` | `float` |  |
| `Class.CylindricalConstraint.MotorMaxAngularAcceleration` | `float` |  |
| `Class.CylindricalConstraint.MotorMaxTorque` | `float` |  |
| `Class.CylindricalConstraint.RotationAxisVisible` | `bool` |  |
| `Class.CylindricalConstraint.ServoMaxTorque` | `float` |  |
| `Class.CylindricalConstraint.SoftlockAngularServoUponReachingTarget` | `bool` | [Deprecated] |
| `Class.CylindricalConstraint.TargetAngle` | `float` |  |
| `Class.CylindricalConstraint.UpperAngle` | `float` |  |
| `Class.CylindricalConstraint.WorldRotationAxis` | `Datatype.Vector3` | [ReadOnly] [NotReplicated] |

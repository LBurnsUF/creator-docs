---
title: BodyGyro
type: class
superclass: BodyMover
tags: [Deprecated]
---

# BodyGyro

Applies a torque to maintain a constant orientation.

**Inherits from:** `Class.BodyMover` > `Class.Instance` > `Class.Object`

**Tags:** [Deprecated]

## Description

The `BodyGyro` object applies a torque (rotational force) on an assembly such
that it maintains a constant angular displacement, or orientation. This allows
for the creation of assemblies that point in a certain direction, as if a real
gyroscope were acting upon it. Essentially, it's the rotational counterpart to
a `Class.BodyPosition`.

If you would like to maintain a constant angular velocity, use a
`Class.BodyAngularVelocity` instead.

The `Class.BodyGyro.CFrame|CFrame` property controls the goal orientation.
Only the angular components of the `Datatype.CFrame` are used; position will
make no difference. `Class.BodyGyro.MaxTorque|MaxTorque` limits the amount of
angular force that may be applied, `Class.BodyGyro.P|P` controls the power
used in achieving the goal orientation, and `Class.BodyGyro.D|D` controls
dampening behavior.

> **Deprecated:** This object is deprecated and should not be used for new work. Use
`Class.AlignOrientation` instead, and see the
[legacy conversion notes](../../../physics/mover-constraints.md#legacy-mover-conversion).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.BodyGyro.CFrame` | `Datatype.CFrame` |  |
| `Class.BodyGyro.D` | `float` |  |
| `Class.BodyGyro.MaxTorque` | `Datatype.Vector3` |  |
| `Class.BodyGyro.P` | `float` |  |
| `Class.BodyGyro.cframe` | `Datatype.CFrame` | [NotReplicated] [Deprecated] |
| `Class.BodyGyro.maxTorque` | `Datatype.Vector3` | [NotReplicated] [Deprecated] |

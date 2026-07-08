---
title: BodyThrust
type: class
superclass: BodyMover
tags: [Deprecated]
---

# BodyThrust

Applies a constant force to an object at a specific point.

**Inherits from:** `Class.BodyMover` > `Class.Instance` > `Class.Object`

**Tags:** [Deprecated]

## Description

The `BodyThrust` object applies a force relative to the assembly to which it
is parented at a specific location. It behaves similar to a `Class.BodyForce`
except that this object's force applies at a specific point
(`Class.BodyThrust.Location|Location`), allowing you to exert a torque
(rotational force). To apply a force dynamically so that an assembly maintains
a constant angular velocity, use a `Class.BodyAngularVelocity` instead. To
apply a force dynamically so that an assembly maintains a constant orientation
(angular position), use a `Class.BodyGyro`.

> **Deprecated:** This object is deprecated and should not be used for new work. Use
`Class.VectorForce` instead, and see the
[legacy conversion notes](../../../physics/mover-constraints.md#legacy-mover-conversion).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.BodyThrust.Force` | `Datatype.Vector3` |  |
| `Class.BodyThrust.Location` | `Datatype.Vector3` |  |
| `Class.BodyThrust.force` | `Datatype.Vector3` | [NotReplicated] [Deprecated] |
| `Class.BodyThrust.location` | `Datatype.Vector3` | [NotReplicated] [Deprecated] |

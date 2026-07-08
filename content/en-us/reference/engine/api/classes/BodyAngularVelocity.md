---
title: BodyAngularVelocity
type: class
superclass: BodyMover
tags: [Deprecated]
---

# BodyAngularVelocity

Applies a torque to maintain a constant angular velocity.

**Inherits from:** `Class.BodyMover` > `Class.Instance` > `Class.Object`

**Tags:** [Deprecated]

## Description

The `BodyAngularVelocity` object applies a torque (rotational force) on an
assembly such that it maintains a constant angular velocity as determined by
its `Class.BodyAngularVelocity.AngularVelocity|AngularVelocity` property. This
allows for the creation of assemblies that continually rotate. It is the
rotational counterpart to a `Class.BodyVelocity`. If you would like to
maintain a constant angular displacement, use a `Class.BodyGyro` instead.

> **Deprecated:** This object is deprecated and should not be used for new work. Use
`Class.AngularVelocity` instead, and see the
[legacy conversion notes](../../../physics/mover-constraints.md#legacy-mover-conversion).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.BodyAngularVelocity.AngularVelocity` | `Datatype.Vector3` |  |
| `Class.BodyAngularVelocity.MaxTorque` | `Datatype.Vector3` |  |
| `Class.BodyAngularVelocity.P` | `float` |  |
| `Class.BodyAngularVelocity.angularvelocity` | `Datatype.Vector3` | [NotReplicated] [Deprecated] |
| `Class.BodyAngularVelocity.maxTorque` | `Datatype.Vector3` | [NotReplicated] [Deprecated] |

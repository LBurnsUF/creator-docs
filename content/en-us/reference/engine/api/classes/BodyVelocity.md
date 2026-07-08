---
title: BodyVelocity
type: class
superclass: BodyMover
tags: [Deprecated]
---

# BodyVelocity

Applies a force to maintain a constant velocity.

**Inherits from:** `Class.BodyMover` > `Class.Instance` > `Class.Object`

**Tags:** [Deprecated]

## Description

The `BodyVelocity` object applies a force on an assembly such that it will
maintain a constant velocity. The `Class.BodyVelocity.Velocity|Velocity`
property, not to be confused with `Class.BasePart.AssemblyLinearVelocity`,
controls the goal velocity.

`Class.BodyVelocity` is the linear counterpart to `Class.BodyAngularVelocity`.
If you need the assembly to move toward a goal position, use
`Class.BodyPosition` instead. If you need further control on a force applied
to an object, consider using a `Class.BodyForce` or `Class.BodyThrust`
instead.

The strength of the force applied by this object is controlled by several
factors, namely the difference between the assembly's current velocity and the
goal velocity. This is multiplied by `Class.BodyVelocity.P|P` (power) to
either amplify or diminish it. The resulting force is then capped by
`Class.BodyVelocity.MaxForce|MaxForce`.

> **Deprecated:** This object is deprecated and should not be used for new work. Use
`Class.LinearVelocity` instead, and see the
[legacy conversion notes](../../../physics/mover-constraints.md#legacy-mover-conversion).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.BodyVelocity.MaxForce` | `Datatype.Vector3` |  |
| `Class.BodyVelocity.P` | `float` |  |
| `Class.BodyVelocity.Velocity` | `Datatype.Vector3` |  |
| `Class.BodyVelocity.maxForce` | `Datatype.Vector3` | [NotReplicated] [Deprecated] |
| `Class.BodyVelocity.velocity` | `Datatype.Vector3` | [NotReplicated] [Deprecated] |

## Methods

### `Class.BodyVelocity:GetLastForce`

``GetLastForce()`` -> `Datatype.Vector3`

### `Class.BodyVelocity:lastForce`

``lastForce()`` -> `Datatype.Vector3`

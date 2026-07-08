---
title: BodyPosition
type: class
superclass: BodyMover
tags: [Deprecated]
---

# BodyPosition

Applies a force to maintain a constant position.

**Inherits from:** `Class.BodyMover` > `Class.Instance` > `Class.Object`

**Tags:** [Deprecated]

## Description

The `BodyPosition` object applies a force on an assembly such that it will
maintain a constant position in the world. The
`Class.BodyPosition.Position|Position` property, not to be confused with
`Class.BasePart.Position`, controls the target world position. This is the
translational counterpart to a `Class.BodyGyro`.

If you need further control on a force applied to an object, consider using a
`Class.BodyForce` or `Class.BodyThrust` instead.

The strength of the force applied by this object is controlled by several
factors, namely the distance to the goal position: the force is stronger when
farther away from the goal. This is amplified by `Class.BodyPosition.P|P`
(power). The present velocity will also dampen the force applied by this
object, and this is amplified by `Class.BodyPosition.D|D` (dampening). The
resulting force is then capped by `Class.BodyPosition.MaxForce|MaxForce`. Note
the force applied on the assembly to achieve the goal position may vary on a
per-axis basis.

> **Deprecated:** This object is deprecated and should not be used for new work. Use
`Class.AlignPosition` instead, and see the
[legacy conversion notes](../../../physics/mover-constraints.md#legacy-mover-conversion).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.BodyPosition.D` | `float` |  |
| `Class.BodyPosition.MaxForce` | `Datatype.Vector3` |  |
| `Class.BodyPosition.P` | `float` |  |
| `Class.BodyPosition.Position` | `Datatype.Vector3` |  |
| `Class.BodyPosition.maxForce` | `Datatype.Vector3` | [NotReplicated] [Deprecated] |
| `Class.BodyPosition.position` | `Datatype.Vector3` | [NotReplicated] [Deprecated] |

## Methods

### `Class.BodyPosition:GetLastForce`

``GetLastForce()`` -> `Datatype.Vector3`

### `Class.BodyPosition:lastForce`

``lastForce()`` -> `Datatype.Vector3`
  [Deprecated]

## Events

### `Class.BodyPosition.ReachedTarget`

Fires with: ()

---
title: RocketPropulsion
type: class
superclass: BodyMover
tags: [Deprecated]
---

# RocketPropulsion

Applies a force so that an assembly follows and faces a target part.

**Inherits from:** `Class.BodyMover` > `Class.Instance` > `Class.Object`

**Tags:** [Deprecated]

## Description

The `RocketPropulsion` object applies force on an assembly so that it both
**follows** and **faces** a target. It acts like a hybrid of
`Class.BodyPosition` and `Class.BodyGyro`. Unlike other
`Class.BodyMover|BodyMovers`, `RocketPropulsion` must be instructed to begin
applying or stopping force via `Class.RocketPropulsion:Fire()|Fire()` or
`Class.RocketPropulsion:Abort()|Abort()` respectively.

You can detect when the assembly reaches its target using the
`Class.RocketPropulsion.ReachedTarget|ReachedTarget` event which fires once
the assembly is within the `Class.RocketPropulsion.TargetRadius|TargetRadius`
of the `Class.RocketPropulsion.Target|Target` part.

> **Deprecated:** This object is deprecated and should not be used for new work. Use
`Class.LineForce` instead, and see the
[legacy conversion notes](../../../physics/mover-constraints.md#legacy-mover-conversion).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.RocketPropulsion.CartoonFactor` | `float` |  |
| `Class.RocketPropulsion.MaxSpeed` | `float` |  |
| `Class.RocketPropulsion.MaxThrust` | `float` |  |
| `Class.RocketPropulsion.MaxTorque` | `Datatype.Vector3` |  |
| `Class.RocketPropulsion.Target` | `Class.BasePart` |  |
| `Class.RocketPropulsion.TargetOffset` | `Datatype.Vector3` |  |
| `Class.RocketPropulsion.TargetRadius` | `float` |  |
| `Class.RocketPropulsion.ThrustD` | `float` |  |
| `Class.RocketPropulsion.ThrustP` | `float` |  |
| `Class.RocketPropulsion.TurnD` | `float` |  |
| `Class.RocketPropulsion.TurnP` | `float` |  |

## Methods

### `Class.RocketPropulsion:Abort`

``Abort()`` -> `null`

### `Class.RocketPropulsion:Fire`

``Fire()`` -> `null`

### `Class.RocketPropulsion:fire`

``fire()`` -> `null`
  [Deprecated]

## Events

### `Class.RocketPropulsion.ReachedTarget`

Fires with: ()

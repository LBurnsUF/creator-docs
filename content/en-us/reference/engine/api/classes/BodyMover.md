---
title: BodyMover
type: class
superclass: Instance
tags: [NotCreatable, Deprecated]
---

# BodyMover

Base class for objects that continually exert forces to assemblies.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Deprecated]

## Description

`BodyMover` is the abstract base class for the set of legacy objects that
exert forces to assemblies in different ways. In general, the subclasses of
`BodyMover` are:

- `Class.BodyForce` exerts a force relative to world coordinates.
- `Class.BodyPosition` exerts force to maintain a certain world position.
- `Class.BodyVelocity` exerts force to maintain a certain velocity.
- `Class.BodyThrust` exerts a force relative to object coordinates which
  applies torque if positioned in a certain way.
- `Class.BodyGyro` exerts torque to maintain a certain orientation.
- `Class.BodyAngularVelocity` exerts torque to maintain a certain angular
  velocity.
- `Class.RocketPropulsion` exerts both translational and rotational forces to
  cause an assembly to track down another.

> **Deprecated:** This class has been deprecated. See the
[mover constraints](../../../physics/mover-constraints.md) article for an
overview of `Class.BodyMover` replacements, as well as the
[legacy conversion notes](../../../physics/mover-constraints.md#legacy-mover-conversion).

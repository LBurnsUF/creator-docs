---
title: BodyForce
type: class
superclass: BodyMover
tags: [Deprecated]
---

# BodyForce

Applies a constant force to an object.

**Inherits from:** `Class.BodyMover` > `Class.Instance` > `Class.Object`

**Tags:** [Deprecated]

## Description

The `BodyForce` object applies (or exerts) a force on the assembly to which it
is parented. If the magnitude of such a force is great enough, assemblies can
begin to accelerate. The force is determined by the
`Class.BodyForce.Force|Force` property, and is defined on the three world
axes.

A `BodyForce` alone cannot apply a torque (it cannot cause the parent to
rotate on its own). To apply a force at a specific point or apply forces
relative to the orientation of the assembly, use a `Class.BodyThrust` instead.

> **Deprecated:** This object is deprecated and should not be used for new work. Use
`Class.VectorForce` instead, and see the
[legacy conversion notes](../../../physics/mover-constraints.md#legacy-mover-conversion).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.BodyForce.Force` | `Datatype.Vector3` |  |
| `Class.BodyForce.force` | `Datatype.Vector3` | [NotReplicated] [Deprecated] |

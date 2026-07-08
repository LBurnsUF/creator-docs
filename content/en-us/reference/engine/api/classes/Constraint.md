---
title: Constraint
type: class
superclass: Instance
tags: [NotCreatable]
---

# Constraint

The base class for constraint-based objects.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

The base class for constraint-based objects. See
[mover constraints](../../../physics/mover-constraints.md) and
[mechanical constraints](../../../physics/mechanical-constraints.md) for more
details.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Constraint.Active` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.Constraint.Attachment0` | `Class.Attachment` |  |
| `Class.Constraint.Attachment1` | `Class.Attachment` |  |
| `Class.Constraint.Color` | `Datatype.BrickColor` |  |
| `Class.Constraint.Enabled` | `bool` |  |
| `Class.Constraint.Visible` | `bool` |  |

## Methods

### `Class.Constraint:GetDebugAppliedForce`

``GetDebugAppliedForce(bodyId: `int`)`` -> `Datatype.Vector3`
  [Deprecated]

### `Class.Constraint:GetDebugAppliedTorque`

``GetDebugAppliedTorque(bodyId: `int`)`` -> `Datatype.Vector3`
  [Deprecated]

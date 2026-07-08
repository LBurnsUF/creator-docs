---
title: Vector3Curve
type: class
superclass: Instance
---

# Vector3Curve

Represents a 3D vector curve, grouping three `Class.FloatCurve` instances.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

Represents a 3D vector curve, grouping three `Class.FloatCurve` instances.
Each child `Class.FloatCurve` can be accessed via the
`Class.Vector3Curve:X()`, `Class.Vector3Curve:Y()`, and
`Class.Vector3Curve:Z()` methods. The three axes can be sampled simultaneously
via the method `Class.Vector3Curve:GetValueAtTime()`.

## Methods

### `Class.Vector3Curve:GetValueAtTime`

``GetValueAtTime(time: `float`)`` -> `Array`

### `Class.Vector3Curve:X`

``X()`` -> `Class.FloatCurve`

### `Class.Vector3Curve:Y`

``Y()`` -> `Class.FloatCurve`

### `Class.Vector3Curve:Z`

``Z()`` -> `Class.FloatCurve`

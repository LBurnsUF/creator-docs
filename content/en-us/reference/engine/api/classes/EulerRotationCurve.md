---
title: EulerRotationCurve
type: class
superclass: Instance
---

# EulerRotationCurve

Represents a 3D rotation curve through a group of three
`Class.FloatCurve|FloatCurves`.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

A **EulerRotationCurve** represents a 3D rotation curve through a group of
three `Class.FloatCurve|FloatCurves`. The rotation is decomposed in three
Euler angles channels that can be accessed via `Class.EulerRotationCurve:X()`,
`Class.EulerRotationCurve:Y()`, and `Class.EulerRotationCurve:Z()`. The three
axes can be sampled simultaneously via
`Class.EulerRotationCurve:GetAnglesAtTime()`, returning the three Euler angles
as a `Datatype.Vector3`. Similarly,
`Class.EulerRotationCurve:GetRotationAtTime()` samples all channels
simultaneously but returns a `Datatype.CFrame` rotated by `X`, `Y`, and `Z`
according to the specified rotation order.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.EulerRotationCurve.RotationOrder` | `Enum.RotationOrder` |  |

## Methods

### `Class.EulerRotationCurve:GetAnglesAtTime`

``GetAnglesAtTime(time: `float`)`` -> `Array`

### `Class.EulerRotationCurve:GetRotationAtTime`

``GetRotationAtTime(time: `float`)`` -> `Datatype.CFrame`

### `Class.EulerRotationCurve:X`

``X()`` -> `Class.FloatCurve`

### `Class.EulerRotationCurve:Y`

``Y()`` -> `Class.FloatCurve`

### `Class.EulerRotationCurve:Z`

``Z()`` -> `Class.FloatCurve`

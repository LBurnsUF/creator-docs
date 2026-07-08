---
title: RotationCurve
type: class
superclass: Instance
---

# RotationCurve

Represents a sequence of rotations and the interpolation curve between them.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

This class holds a sorted list of
`Datatype.RotationCurveKey|RotationCurveKeys` that represent a sequence of
rotations. The shape of the interpolation curve between two keys is determined
by the `Datatype.RotationCurveKey.Interpolation` type.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.RotationCurve.Length` | `int` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.RotationCurve:GetKeyAtIndex`

``GetKeyAtIndex(index: `int`)`` -> `Datatype.RotationCurveKey`

### `Class.RotationCurve:GetKeyIndicesAtTime`

``GetKeyIndicesAtTime(time: `float`)`` -> `Array`

### `Class.RotationCurve:GetKeys`

``GetKeys()`` -> `Array`

### `Class.RotationCurve:GetValueAtTime`

``GetValueAtTime(time: `float`)`` -> `Datatype.CoordinateFrame`?

### `Class.RotationCurve:InsertKey`

``InsertKey(key: `Datatype.RotationCurveKey`)`` -> `Array`

### `Class.RotationCurve:RemoveKeyAtIndex`

``RemoveKeyAtIndex(startingIndex: `int`, count: `int`)`` -> `int`

### `Class.RotationCurve:SetKeys`

``SetKeys(keys: `Array`)`` -> `int`

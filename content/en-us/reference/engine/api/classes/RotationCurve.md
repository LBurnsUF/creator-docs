---
title: RotationCurve
type: class
superclass: Instance
---

# RotationCurve

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.RotationCurve.Length` | `int` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.RotationCurve:GetKeyAtIndex`

``GetKeyAtIndex(index: `int`)`` → `Datatype.RotationCurveKey`

### `Class.RotationCurve:GetKeyIndicesAtTime`

``GetKeyIndicesAtTime(time: `float`)`` → `Array`

### `Class.RotationCurve:GetKeys`

``GetKeys()`` → `Array`

### `Class.RotationCurve:GetValueAtTime`

``GetValueAtTime(time: `float`)`` → `Datatype.CoordinateFrame`?

### `Class.RotationCurve:InsertKey`

``InsertKey(key: `Datatype.RotationCurveKey`)`` → `Array`

### `Class.RotationCurve:RemoveKeyAtIndex`

``RemoveKeyAtIndex(startingIndex: `int`, count: `int`)`` → `int`

### `Class.RotationCurve:SetKeys`

``SetKeys(keys: `Array`)`` → `int`

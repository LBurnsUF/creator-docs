---
title: FloatCurve
type: class
superclass: Instance
---

# FloatCurve

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.FloatCurve.Length` | `int` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.FloatCurve:GetKeyAtIndex`

``GetKeyAtIndex(index: `int`)`` → `Datatype.FloatCurveKey`

### `Class.FloatCurve:GetKeyIndicesAtTime`

``GetKeyIndicesAtTime(time: `float`)`` → `Array`

### `Class.FloatCurve:GetKeys`

``GetKeys()`` → `Array`

### `Class.FloatCurve:GetValueAtTime`

``GetValueAtTime(time: `float`)`` → `float?`

### `Class.FloatCurve:InsertKey`

``InsertKey(key: `Datatype.FloatCurveKey`)`` → `Array`

### `Class.FloatCurve:RemoveKeyAtIndex`

``RemoveKeyAtIndex(startingIndex: `int`, count: `int`)`` → `int`

### `Class.FloatCurve:SetKeys`

``SetKeys(keys: `Array`)`` → `int`

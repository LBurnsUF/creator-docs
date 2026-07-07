---
title: ValueCurve
type: class
superclass: Instance
---

# ValueCurve

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.ValueCurve.Length` | `int` | [ReadOnly] [NotReplicated] |
| `Class.ValueCurve.ValueType` | `string` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.ValueCurve:GetKeyAtIndex`

``GetKeyAtIndex(index: `int`)`` → `Datatype.ValueCurveKey`

### `Class.ValueCurve:GetKeyIndicesAtTime`

``GetKeyIndicesAtTime(time: `float`)`` → `Array`

### `Class.ValueCurve:GetKeys`

``GetKeys()`` → `Array`

### `Class.ValueCurve:GetValueAtTime`

``GetValueAtTime(time: `float`)`` → `Variant?`

### `Class.ValueCurve:InsertKey`

``InsertKey(key: `Datatype.ValueCurveKey`)`` → `Array`

### `Class.ValueCurve:InsertKeyValue`

``InsertKeyValue(time: `float`, value: `Variant`, keyInterpolationMode: `Enum.KeyInterpolationMode`)`` → `Array`

### `Class.ValueCurve:RemoveKeyAtIndex`

``RemoveKeyAtIndex(startingIndex: `int`, count: `int`)`` → `int`

### `Class.ValueCurve:SetKeys`

``SetKeys(keys: `Array`)`` → `int`

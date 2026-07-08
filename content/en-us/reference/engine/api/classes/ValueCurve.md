---
title: ValueCurve
type: class
superclass: Instance
---

# ValueCurve

A sorted list of time-value pairs that define a curve. Used to animate a any
type of value.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

An instance representing a 1D value curve encoded via a sorted list of
`Datatype.ValueCurveKey|ValueCurveKeys`. The shape of the interpolation curve
between two keys is determined by the `Datatype.ValueCurveKey.Interpolation`
type.

Not all value types (for example, strings and other non-numerical types) may
perform `Enum.KeyInterpolationMode.Linear|Linear` or
`Enum.KeyInterpolationMode.Cubic|Cubic` interpolation. These types will revert
to `Enum.KeyInterpolationMode.Constant|Constant` interpolation if necessary.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ValueCurve.Length` | `int` | [ReadOnly] [NotReplicated] |
| `Class.ValueCurve.ValueType` | `string` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.ValueCurve:GetKeyAtIndex`

``GetKeyAtIndex(index: `int`)`` -> `Datatype.ValueCurveKey`

### `Class.ValueCurve:GetKeyIndicesAtTime`

``GetKeyIndicesAtTime(time: `float`)`` -> `Array`

### `Class.ValueCurve:GetKeys`

``GetKeys()`` -> `Array`

### `Class.ValueCurve:GetValueAtTime`

``GetValueAtTime(time: `float`)`` -> `Variant?`

### `Class.ValueCurve:InsertKey`

``InsertKey(key: `Datatype.ValueCurveKey`)`` -> `Array`

### `Class.ValueCurve:InsertKeyValue`

``InsertKeyValue(time: `float`, value: `Variant`, keyInterpolationMode: `Enum.KeyInterpolationMode`)`` -> `Array`

### `Class.ValueCurve:RemoveKeyAtIndex`

``RemoveKeyAtIndex(startingIndex: `int`, count: `int`)`` -> `int`

### `Class.ValueCurve:SetKeys`

``SetKeys(keys: `Array`)`` -> `int`

---
title: FloatCurve
type: class
superclass: Instance
---

# FloatCurve

A sorted list of time-value pairs that define a curve. Used to animate a
single numerical value.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

An instance representing a 1D float curve encoded via a sorted list of
`Datatype.FloatCurveKey|FloatCurveKeys`. The shape of the interpolation curve
between two keys is determined by the `Datatype.FloatCurveKey.Interpolation`
type.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.FloatCurve.Length` | `int` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.FloatCurve:GetKeyAtIndex`

``GetKeyAtIndex(index: `int`)`` -> `Datatype.FloatCurveKey`

### `Class.FloatCurve:GetKeyIndicesAtTime`

``GetKeyIndicesAtTime(time: `float`)`` -> `Array`

### `Class.FloatCurve:GetKeys`

``GetKeys()`` -> `Array`

### `Class.FloatCurve:GetValueAtTime`

``GetValueAtTime(time: `float`)`` -> `float?`

### `Class.FloatCurve:InsertKey`

``InsertKey(key: `Datatype.FloatCurveKey`)`` -> `Array`

### `Class.FloatCurve:RemoveKeyAtIndex`

``RemoveKeyAtIndex(startingIndex: `int`, count: `int`)`` -> `int`

### `Class.FloatCurve:SetKeys`

``SetKeys(keys: `Array`)`` -> `int`

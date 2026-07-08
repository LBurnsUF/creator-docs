---
title: FloatCurveKey
type: datatype
---

# `Datatype.FloatCurveKey`

A time-value pair used with `Class.FloatCurve` instances.

## Description

A time-value pair used with `Class.FloatCurve` instances.

The `Datatype.FloatCurveKey.Interpolation|Interpolation` property dictates the
interpolation mode for the segment started by this key and ended by the next
key on the curve. Each segment may use a different interpolation mode.

The `Datatype.FloatCurveKey.LeftTangent|LeftTangent` and
`Datatype.FloatCurveKey.RightTangent|RightTangent` properties apply to the
cubic interpolation mode and define the desired tangent (slope) at the key.
Different left and right values can be used to encode discontinuities in slope
at the key. Attempting to set a
`Datatype.FloatCurveKey.RightTangent|RightTangent` value on a key that doesn't
use the cubic interpolation mode will result in a runtime error. It is
possible to set the `Datatype.FloatCurveKey.LeftTangent|LeftTangent` property
on any key, as it will be used should the preceding segment use cubic
interpolation.

## Constructors

### `FloatCurveKey.new`

Creates a new `Datatype.FloatCurveKey` at a given time and value.
`Datatype.FloatCurveKey.LeftTangent|LeftTangent` and
`Datatype.FloatCurveKey.RightTangent|RightTangent` are left uninitialized
and, if not initialized, tangent values of 0 will be used when evaluating
the curve.

**Parameters:**

- `time`: `number` - Time at which to create the new `Datatype.FloatCurveKey`.
- `value`: `number` - Value of the new `Datatype.FloatCurveKey`.
- `Interpolation`: `KeyInterpolationMode`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `FloatCurveKey.Interpolation` | `KeyInterpolationMode` | The key interpolation mode for the segment started by this `Datatype.FloatCurveKey`. |
| `FloatCurveKey.Time` | `number` | The time position of this `Datatype.FloatCurveKey`. |
| `FloatCurveKey.Value` | `number` | The value of this `Datatype.FloatCurveKey`. |
| `FloatCurveKey.RightTangent` | `number` | The tangent to the right of this `Datatype.FloatCurveKey`. |
| `FloatCurveKey.LeftTangent` | `number` | The tangent to the left of this `Datatype.FloatCurveKey`. |

## API Usage (2 locations)

### Used as Parameter Type

- `Class.FloatCurve:InsertKey` (parameter `key`)

### Used as Return Type

- `Class.FloatCurve:GetKeyAtIndex`

---
title: ValueCurveKey
type: datatype
---

# `Datatype.ValueCurveKey`

A time-value pair used with `Class.ValueCurve` instances.

## Description

A time-value pair used with `Class.ValueCurve` instances.

The `Datatype.ValueCurveKey.Interpolation|Interpolation` property dictates the
interpolation mode for the segment started by this key and ended by the next
key on the curve. Each segment may use a different interpolation mode.

The `Datatype.ValueCurveKey.LeftTangent|LeftTangent` and
`Datatype.ValueCurveKey.RightTangent|RightTangent` properties apply to the
cubic interpolation mode and define the desired tangent (slope) at the key.
Different left and right values can be used to encode discontinuities in slope
at the key. Attempting to set a
`Datatype.ValueCurveKey.RightTangent|RightTangent` value on a key that doesn't
use the cubic interpolation mode will result in a runtime error. It is
possible to set the `Datatype.ValueCurveKey.LeftTangent|LeftTangent` property
on any key, as it will be used should the preceding segment use cubic
interpolation.

## Constructors

### `ValueCurveKey.new`

Creates a new `Datatype.ValueCurveKey` at a given time and value.
`Datatype.ValueCurveKey.LeftTangent|LeftTangent` and
`Datatype.ValueCurveKey.RightTangent|RightTangent` are left uninitialized
and, if not initialized, tangent values of '0' will be used when evaluating
the curve.

**Parameters:**

- `time`: `number` - Time at which to create the new `Datatype.ValueCurveKey`.
- `value`: `any` - Value of the new `Datatype.ValueCurveKey`.
- `Interpolation`: `KeyInterpolationMode`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `ValueCurveKey.Interpolation` | `KeyInterpolationMode` | The key interpolation mode for the segment started by this `Datatype.ValueCurveKey`. |
| `ValueCurveKey.Time` | `number` | The time position of this `Datatype.ValueCurveKey`. |
| `ValueCurveKey.Value` | `any` | The value of this `Datatype.ValueCurveKey`. |
| `ValueCurveKey.RightTangent` | `number` | The tangent to the right of this `Datatype.ValueCurveKey`. |
| `ValueCurveKey.LeftTangent` | `number` | The tangent to the left of this `Datatype.ValueCurveKey`. |

## API Usage (2 locations)

### Used as Parameter Type

- `Class.ValueCurve:InsertKey` (parameter `key`)

### Used as Return Type

- `Class.ValueCurve:GetKeyAtIndex`

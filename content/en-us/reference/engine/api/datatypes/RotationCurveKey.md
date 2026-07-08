---
title: RotationCurveKey
type: datatype
---

# `Datatype.RotationCurveKey`

A time-value pair used with `Class.RotationCurve` instances.

## Description

A time-value pair used with `Class.RotationCurve` instances.

The `Datatype.RotationCurveKey.Interpolation|Interpolation` property dictates
the interpolation mode for the segment started by this key and ended by the
next key on the curve. Each segment may use a different interpolation mode.

The `Datatype.RotationCurveKey.LeftTangent|LeftTangent` and
`Datatype.RotationCurveKey.RightTangent|RightTangent` properties apply to the
cubic interpolation mode and define the desired tangent (slope) at the key.
Different left and right values can be used to encode discontinuities in slope
at the key. Attempting to set a
`Datatype.RotationCurveKey.RightTangent|RightTangent` value on a key that
doesn't use the cubic interpolation mode will result in a runtime error. It is
possible to set the `Datatype.RotationCurveKey.LeftTangent|LeftTangent`
property on any key, as it will be used should the preceding segment use cubic
interpolation.

## Constructors

### `RotationCurveKey.new`

Creates a new `Datatype.RotationCurveKey` at a given time with a given
`Datatype.CFrame`. `Datatype.RotationCurveKey.LeftTangent|LeftTangent` and
`Datatype.RotationCurveKey.RightTangent|RightTangent` are left
uninitialized and, if not initialized, tangent values of 0 will be used
when evaluating the curve.

**Parameters:**

- `time`: `number` - Time at which to create the new `Datatype.RotationCurveKey`.
- `cframe`: `CFrame` - `Datatype.CFrame` of the new `Datatype.RotationCurveKey`.
- `Interpolation`: `KeyInterpolationMode`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `RotationCurveKey.Interpolation` | `KeyInterpolationMode` | The key interpolation mode for the segment started by this `Datatype.RotationCurveKey`. |
| `RotationCurveKey.Time` | `number` | The time position of this `Datatype.RotationCurveKey`. |
| `RotationCurveKey.Value` | `CFrame` | The `Datatype.CFrame` value of this `Datatype.RotationCurveKey`. |
| `RotationCurveKey.RightTangent` | `number` | The tangent to the right of this `Datatype.RotationCurveKey`. |
| `RotationCurveKey.LeftTangent` | `number` | The tangent to the left of this `Datatype.RotationCurveKey`. |

## API Usage (2 locations)

### Used as Parameter Type

- `Class.RotationCurve:InsertKey` (parameter `key`)

### Used as Return Type

- `Class.RotationCurve:GetKeyAtIndex`

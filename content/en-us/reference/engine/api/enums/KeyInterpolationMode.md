---
title: KeyInterpolationMode
type: enum
---

# `Enum.KeyInterpolationMode`

Describes the interpolation method between two keys.

Describes the interpolation method for a `Class.FloatCurve` or
`Class.RotationCurve` segment between the key for which this mode is set and
the next key in the curve.

The `Enum.KeyInterpolationMode` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.KeyInterpolationMode.Constant` | 0 | The segment starting at this key will constantly evaluate to the value set at this key. |
| `Enum.KeyInterpolationMode.Linear` | 1 | The segment starting at this key will evaluate using a linear interpolation at this key and the valu |
| `Enum.KeyInterpolationMode.Cubic` | 2 | The segment starting at this key will evaluate using cubic interpolation of this key value using its |

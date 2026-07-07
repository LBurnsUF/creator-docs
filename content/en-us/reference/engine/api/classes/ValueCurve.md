---
title: ValueCurve
type: class
superclass: Instance
---

# ValueCurve

**Inherits**: Instance > Object

## Properties

- **Length**: `int` [ReadOnly] [NotReplicated]
- **ValueType**: `string` [ReadOnly] [NotReplicated]

## Methods

- **GetKeyAtIndex**(`index: int`) -> `ValueCurveKey`
- **GetKeyIndicesAtTime**(`time: float`) -> `Array`
- **GetKeys**() -> `Array`
- **GetValueAtTime**(`time: float`) -> `Variant?`
- **InsertKey**(`key: ValueCurveKey`) -> `Array`
- **InsertKeyValue**(`time: float`, `value: Variant`, `keyInterpolationMode: KeyInterpolationMode = Constant`) -> `Array`
- **RemoveKeyAtIndex**(`startingIndex: int`, `count: int = 1`) -> `int`
- **SetKeys**(`keys: Array`) -> `int`

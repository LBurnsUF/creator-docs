---
title: FloatCurve
type: class
superclass: Instance
---

# FloatCurve

**Inherits**: Instance > Object

## Properties

- **Length**: `int` [ReadOnly] [NotReplicated]

## Methods

- **GetKeyAtIndex**(`index: int`) -> `FloatCurveKey`
- **GetKeyIndicesAtTime**(`time: float`) -> `Array`
- **GetKeys**() -> `Array`
- **GetValueAtTime**(`time: float`) -> `float?`
- **InsertKey**(`key: FloatCurveKey`) -> `Array`
- **RemoveKeyAtIndex**(`startingIndex: int`, `count: int = 1`) -> `int`
- **SetKeys**(`keys: Array`) -> `int`

---
title: RotationCurve
type: class
superclass: Instance
---

# RotationCurve

**Inherits**: Instance > Object

## Properties

- **Length**: `int` [ReadOnly] [NotReplicated]

## Methods

- **GetKeyAtIndex**(`index: int`) -> `RotationCurveKey`
- **GetKeyIndicesAtTime**(`time: float`) -> `Array`
- **GetKeys**() -> `Array`
- **GetValueAtTime**(`time: float`) -> `CoordinateFrame?`
- **InsertKey**(`key: RotationCurveKey`) -> `Array`
- **RemoveKeyAtIndex**(`startingIndex: int`, `count: int = 1`) -> `int`
- **SetKeys**(`keys: Array`) -> `int`

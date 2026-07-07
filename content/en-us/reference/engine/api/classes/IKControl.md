---
title: IKControl
type: class
superclass: Instance
---

# IKControl

**Inherits**: Instance > Object

## Properties

- **ChainRoot**: `Instance`
- **Enabled**: `bool`
- **EndEffector**: `Instance`
- **EndEffectorOffset**: `CFrame`
- **Offset**: `CFrame`
- **Pole**: `Instance`
- **Priority**: `int`
- **SmoothTime**: `float`
- **Target**: `Instance`
- **Type**: `IKControlType`
- **Weight**: `float`

## Methods

- **GetChainCount**() -> `int`
- **GetChainLength**() -> `float`
- **GetNodeLocalCFrame**(`index: int`) -> `CFrame`
- **GetNodeWorldCFrame**(`index: int`) -> `CFrame`
- **GetRawFinalTarget**() -> `CFrame`
- **GetSmoothedFinalTarget**() -> `CFrame`
- **Solve**() -> `null`

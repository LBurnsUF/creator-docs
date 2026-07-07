---
title: AudioReverb
type: class
superclass: Instance
---

# AudioReverb

**Inherits**: Instance > Object

## Properties

- **Bypass**: `bool`
- **DecayRatio**: `float`
- **DecayTime**: `float`
- **Density**: `float`
- **Diffusion**: `float`
- **DryLevel**: `float`
- **EarlyDelayTime**: `float`
- **HighCutFrequency**: `float`
- **LateDelayTime**: `float`
- **LowShelfFrequency**: `float`
- **LowShelfGain**: `float`
- **ReferenceFrequency**: `float`
- **WetLevel**: `float`

## Methods

- **GetConnectedWires**(`pin: string`) -> `Instances`
- **GetInputPins**() -> `Array`
- **GetOutputPins**() -> `Array`
- **Reset**() -> `null`

## Events

- **WiringChanged**(`connected: bool`, `pin: string`, `wire: Wire`, `instance: Instance`)

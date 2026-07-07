---
title: AudioEcho
type: class
superclass: Instance
---

# AudioEcho

**Inherits**: Instance > Object

## Properties

- **Bypass**: `bool`
- **DelayTime**: `float`
- **DryLevel**: `float`
- **Feedback**: `float`
- **RampTime**: `float`
- **WetLevel**: `float`

## Methods

- **GetConnectedWires**(`pin: string`) -> `Instances`
- **GetInputPins**() -> `Array`
- **GetOutputPins**() -> `Array`
- **Reset**() -> `null`

## Events

- **WiringChanged**(`connected: bool`, `pin: string`, `wire: Wire`, `instance: Instance`)

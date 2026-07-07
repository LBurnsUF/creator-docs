---
title: AudioGate
type: class
superclass: Instance
---

# AudioGate

**Inherits**: Instance > Object

## Properties

- **Attack**: `float`
- **Bypass**: `bool`
- **Release**: `float`
- **Threshold**: `NumberRange`

## Methods

- **GetConnectedWires**(`pin: string`) -> `Instances`
- **GetInputPins**() -> `Array`
- **GetOutputPins**() -> `Array`
- **Reset**() -> `null`

## Events

- **WiringChanged**(`connected: bool`, `pin: string`, `wire: Wire`, `instance: Instance`)

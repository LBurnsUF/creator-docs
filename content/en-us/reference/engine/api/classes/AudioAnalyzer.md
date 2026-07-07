---
title: AudioAnalyzer
type: class
superclass: Instance
---

# AudioAnalyzer

**Inherits**: Instance > Object

## Properties

- **PeakLevel**: `float` [ReadOnly] [NotReplicated]
- **RmsLevel**: `float` [ReadOnly] [NotReplicated]
- **SpectrumEnabled**: `bool`
- **WindowSize**: `AudioWindowSize`

## Methods

- **GetConnectedWires**(`pin: string`) -> `Instances`
- **GetInputPins**() -> `Array`
- **GetOutputPins**() -> `Array`
- **GetSpectrum**() -> `Array` [CustomLuaState]

## Events

- **WiringChanged**(`connected: bool`, `pin: string`, `wire: Wire`, `instance: Instance`)

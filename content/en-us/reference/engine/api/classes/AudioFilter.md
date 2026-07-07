---
title: AudioFilter
type: class
superclass: Instance
---

# AudioFilter

**Inherits**: Instance > Object

## Properties

- **Bypass**: `bool`
- **Editor**: `bool` [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **FilterType**: `AudioFilterType`
- **Frequency**: `float`
- **Gain**: `float`
- **Q**: `float`

## Methods

- **GetConnectedWires**(`pin: string`) -> `Instances`
- **GetGainAt**(`frequency: float`) -> `float`
- **GetInputPins**() -> `Array`
- **GetOutputPins**() -> `Array`

## Events

- **WiringChanged**(`connected: bool`, `pin: string`, `wire: Wire`, `instance: Instance`)

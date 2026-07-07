---
title: AudioEqualizer
type: class
superclass: Instance
---

# AudioEqualizer

**Inherits**: Instance > Object

## Properties

- **Bypass**: `bool`
- **Editor**: `bool` [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **HighGain**: `float`
- **LowGain**: `float`
- **MidGain**: `float`
- **MidRange**: `NumberRange`

## Methods

- **GetConnectedWires**(`pin: string`) -> `Instances`
- **GetInputPins**() -> `Array`
- **GetOutputPins**() -> `Array`

## Events

- **WiringChanged**(`connected: bool`, `pin: string`, `wire: Wire`, `instance: Instance`)

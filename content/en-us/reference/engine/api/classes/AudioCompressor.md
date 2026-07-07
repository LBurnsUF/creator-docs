---
title: AudioCompressor
type: class
superclass: Instance
---

# AudioCompressor

**Inherits**: Instance > Object

## Properties

- **Attack**: `float`
- **Bypass**: `bool`
- **Editor**: `bool` [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **MakeupGain**: `float`
- **Ratio**: `float`
- **Release**: `float`
- **Threshold**: `float`

## Methods

- **GetConnectedWires**(`pin: string`) -> `Instances`
- **GetInputPins**() -> `Array`
- **GetOutputPins**() -> `Array`

## Events

- **WiringChanged**(`connected: bool`, `pin: string`, `wire: Wire`, `instance: Instance`)

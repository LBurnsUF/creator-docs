---
title: AudioLimiter
type: class
superclass: Instance
---

# AudioLimiter

**Inherits**: Instance > Object

## Properties

- **Bypass**: `bool`
- **Editor**: `bool` [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **MaxLevel**: `float`
- **Release**: `float`

## Methods

- **GetConnectedWires**(`pin: string`) -> `Instances`
- **GetInputPins**() -> `Array`
- **GetOutputPins**() -> `Array`

## Events

- **WiringChanged**(`connected: bool`, `pin: string`, `wire: Wire`, `instance: Instance`)

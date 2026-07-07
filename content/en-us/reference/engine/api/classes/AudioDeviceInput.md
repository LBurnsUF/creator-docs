---
title: AudioDeviceInput
type: class
superclass: Instance
---

# AudioDeviceInput

**Inherits**: Instance > Object

## Properties

- **AccessType**: `AccessModifierType`
- **Active**: `bool` (Security: Read=None, Write=RobloxScriptSecurity)
- **EchoCancellation**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **GainControl**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **IsReady**: `bool` [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Muted**: `bool`
- **MutedByLocalUser**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **NoiseSuppression**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Player**: `Player`
- **Volume**: `float`

## Methods

- **GetConnectedWires**(`pin: string`) -> `Instances`
- **GetInputPins**() -> `Array`
- **GetOutputPins**() -> `Array`
- **GetUserIdAccessList**() -> `Array`
- **SetUserIdAccessList**(`userIds: Array`) -> `null`

## Events

- **WiringChanged**(`connected: bool`, `pin: string`, `wire: Wire`, `instance: Instance`)

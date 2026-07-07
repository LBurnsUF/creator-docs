---
title: RealtimeMedia
type: class
superclass: Instance
---

# RealtimeMedia

**Inherits**: Instance > Object

## Properties

- **ForwardInput**: `bool` (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **IsConnected**: `bool` [ReadOnly] [NotReplicated]

## Methods

- **ConnectAsync**(`serverUrl: string`, `connectParams: Dictionary = nil`) -> `bool` [Yields]
- **Disconnect**() -> `null`
- **GetConnectedWires**(`pin: string`) -> `Instances`
- **GetInputPins**() -> `Array`
- **GetOutputPins**() -> `Array`
- **SendMessage**(`message: string`, `binary: bool`) -> `bool`

## Events

- **OnMessage**(`message: string`, `binary: bool`)
- **WiringChanged**(`connected: bool`, `pin: string`, `wire: Wire`, `instance: Instance`)

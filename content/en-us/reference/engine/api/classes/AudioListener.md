---
title: AudioListener
type: class
superclass: Instance
---

# AudioListener

**Inherits**: Instance > Object

## Properties

- **AcousticSimulationEnabled**: `bool`
- **AngleAttenuation**: `BinaryString` (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **AudioInteractionGroup**: `string`
- **DiffractionEnabled**: `SimulationMode`
- **DistanceAttenuation**: `BinaryString` (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **OcclusionEnabled**: `SimulationMode`
- **PositionInstance**: `Instance`
- **PositionType**: `ListenerPositionType`
- **ReverbEnabled**: `SimulationMode`
- **SimulationFidelity**: `AudioSimulationFidelity` [Deprecated]

## Methods

- **GetAngleAttenuation**() -> `Dictionary` [CustomLuaState]
- **GetAudibilityFor**(`emitter: AudioEmitter`) -> `float`
- **GetConnectedWires**(`pin: string`) -> `Instances`
- **GetDistanceAttenuation**() -> `Dictionary` [CustomLuaState]
- **GetInputPins**() -> `Array`
- **GetInteractingEmitters**() -> `Instances`
- **GetOutputPins**() -> `Array`
- **Reset**() -> `null`
- **SetAngleAttenuation**(`curve: Dictionary`) -> `null` [CustomLuaState]
- **SetDistanceAttenuation**(`curve: Dictionary`) -> `null` [CustomLuaState]

## Events

- **WiringChanged**(`connected: bool`, `pin: string`, `wire: Wire`, `instance: Instance`)

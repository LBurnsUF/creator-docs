---
title: AudioEmitter
type: class
superclass: Instance
---

# AudioEmitter

**Inherits**: Instance > Object

## Properties

- **AcousticSimulationEnabled**: `bool`
- **AngleAttenuation**: `BinaryString` (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **AudioInteractionGroup**: `string`
- **DiffractionEnabled**: `SimulationMode`
- **DistanceAttenuation**: `BinaryString` (Security: Read=RobloxSecurity, Write=RobloxSecurity)
- **OcclusionEnabled**: `SimulationMode`
- **PositionInstance**: `Instance`
- **PositionType**: `EmitterPositionType`
- **ReverbEnabled**: `SimulationMode`
- **SimulationFidelity**: `AudioSimulationFidelity` [Deprecated]

## Methods

- **GetAngleAttenuation**() -> `Dictionary` [CustomLuaState]
- **GetAudibilityFor**(`listener: AudioListener`) -> `float`
- **GetConnectedWires**(`pin: string`) -> `Instances`
- **GetDistanceAttenuation**() -> `Dictionary` [CustomLuaState]
- **GetInputPins**() -> `Array`
- **GetInteractingListeners**() -> `Instances`
- **GetOutputPins**() -> `Array`
- **SetAngleAttenuation**(`curve: Dictionary`) -> `null` [CustomLuaState]
- **SetDistanceAttenuation**(`curve: Dictionary`) -> `null` [CustomLuaState]

## Events

- **WiringChanged**(`connected: bool`, `pin: string`, `wire: Wire`, `instance: Instance`)

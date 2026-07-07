---
title: AudioListener
type: class
superclass: Instance
---

# AudioListener

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.AudioListener.AcousticSimulationEnabled` | `bool` |  |
| `Class.AudioListener.AngleAttenuation` | `Datatype.BinaryString` |  {security: RobloxSecurity} |
| `Class.AudioListener.AudioInteractionGroup` | `string` |  |
| `Class.AudioListener.DiffractionEnabled` | `Enum.SimulationMode` |  |
| `Class.AudioListener.DistanceAttenuation` | `Datatype.BinaryString` |  {security: RobloxSecurity} |
| `Class.AudioListener.OcclusionEnabled` | `Enum.SimulationMode` |  |
| `Class.AudioListener.PositionInstance` | `Class.Instance` |  |
| `Class.AudioListener.PositionType` | `Enum.ListenerPositionType` |  |
| `Class.AudioListener.ReverbEnabled` | `Enum.SimulationMode` |  |
| `Class.AudioListener.SimulationFidelity` | `Enum.AudioSimulationFidelity` | [Deprecated] |

## Methods

### `Class.AudioListener:GetAngleAttenuation`

``GetAngleAttenuation()`` → `Dictionary`
  [CustomLuaState]

### `Class.AudioListener:GetAudibilityFor`

``GetAudibilityFor(emitter: `Class.AudioEmitter`)`` → `float`

### `Class.AudioListener:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` → `Datatype.Instances`

### `Class.AudioListener:GetDistanceAttenuation`

``GetDistanceAttenuation()`` → `Dictionary`
  [CustomLuaState]

### `Class.AudioListener:GetInputPins`

``GetInputPins()`` → `Array`

### `Class.AudioListener:GetInteractingEmitters`

``GetInteractingEmitters()`` → `Datatype.Instances`

### `Class.AudioListener:GetOutputPins`

``GetOutputPins()`` → `Array`

### `Class.AudioListener:Reset`

``Reset()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AudioListener:SetAngleAttenuation`

``SetAngleAttenuation(curve: `Dictionary`)`` → `null`
  [CustomLuaState]

### `Class.AudioListener:SetDistanceAttenuation`

``SetDistanceAttenuation(curve: `Dictionary`)`` → `null`
  [CustomLuaState]

## Events

### `Class.AudioListener.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

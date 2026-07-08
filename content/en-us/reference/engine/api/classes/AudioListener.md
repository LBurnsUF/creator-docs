---
title: AudioListener
type: class
superclass: Instance
---

# AudioListener

Records an audio stream from its surrounding
`Class.AudioEmitter|AudioEmitters` in the 3D world.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.AudioListener` records an audio stream from its surrounding
`Class.AudioEmitter|AudioEmitters` in the 3D world. It provides a single
**Output** pin which can be connected to other pins via `Class.Wire|Wires`. If
the parent is an `Class.Attachment`, `Class.Camera`, or `Class.PVInstance`,
the parent's world `Datatype.CFrame` will be used for listening. If the parent
is not one of these classes, the `Class.AudioListener` effectively hears
nothing.

## Properties

| Property | Type | Description |
|----------|------|-------------|
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

``GetAngleAttenuation()`` -> `Dictionary`
  [CustomLuaState]

### `Class.AudioListener:GetAudibilityFor`

``GetAudibilityFor(emitter: `Class.AudioEmitter`)`` -> `float`

### `Class.AudioListener:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioListener:GetDistanceAttenuation`

``GetDistanceAttenuation()`` -> `Dictionary`
  [CustomLuaState]

### `Class.AudioListener:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.AudioListener:GetInteractingEmitters`

``GetInteractingEmitters()`` -> `Datatype.Instances`

### `Class.AudioListener:GetOutputPins`

``GetOutputPins()`` -> `Array`

### `Class.AudioListener:Reset`

``Reset()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AudioListener:SetAngleAttenuation`

``SetAngleAttenuation(curve: `Dictionary`)`` -> `null`
  [CustomLuaState]

### `Class.AudioListener:SetDistanceAttenuation`

``SetDistanceAttenuation(curve: `Dictionary`)`` -> `null`
  [CustomLuaState]

## Events

### `Class.AudioListener.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

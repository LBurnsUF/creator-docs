---
title: AudioEmitter
type: class
superclass: Instance
---

# AudioEmitter

Emits audio streams into the world.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.AudioEmitter` emits audio streams into the world. It provides a single
**Input** pin that can be connected to by one or more `Class.Wire|Wires`. Any
streams wired to an `Class.AudioEmitter` get broadcasted into the world from
the emitter's parent's position. If the parent is an `Class.Attachment`,
`Class.Camera`, or `Class.PVInstance`, the parent's world-position will be
used. If the parent is not one of these classes, the `Class.AudioEmitter` is
effectively silent.

`Class.AudioEmitter|AudioEmitters` are heard by
`Class.AudioListener|AudioListeners` in order to implement 3D spatialization.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioEmitter.AcousticSimulationEnabled` | `bool` |  |
| `Class.AudioEmitter.AngleAttenuation` | `Datatype.BinaryString` |  {security: RobloxSecurity} |
| `Class.AudioEmitter.AudioInteractionGroup` | `string` |  |
| `Class.AudioEmitter.DiffractionEnabled` | `Enum.SimulationMode` |  |
| `Class.AudioEmitter.DistanceAttenuation` | `Datatype.BinaryString` |  {security: RobloxSecurity} |
| `Class.AudioEmitter.OcclusionEnabled` | `Enum.SimulationMode` |  |
| `Class.AudioEmitter.PositionInstance` | `Class.Instance` |  |
| `Class.AudioEmitter.PositionType` | `Enum.EmitterPositionType` |  |
| `Class.AudioEmitter.ReverbEnabled` | `Enum.SimulationMode` |  |
| `Class.AudioEmitter.SimulationFidelity` | `Enum.AudioSimulationFidelity` | [Deprecated] |

## Methods

### `Class.AudioEmitter:GetAngleAttenuation`

``GetAngleAttenuation()`` -> `Dictionary`
  [CustomLuaState]

### `Class.AudioEmitter:GetAudibilityFor`

``GetAudibilityFor(listener: `Class.AudioListener`)`` -> `float`

### `Class.AudioEmitter:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioEmitter:GetDistanceAttenuation`

``GetDistanceAttenuation()`` -> `Dictionary`
  [CustomLuaState]

### `Class.AudioEmitter:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.AudioEmitter:GetInteractingListeners`

``GetInteractingListeners()`` -> `Datatype.Instances`

### `Class.AudioEmitter:GetOutputPins`

``GetOutputPins()`` -> `Array`

### `Class.AudioEmitter:SetAngleAttenuation`

``SetAngleAttenuation(curve: `Dictionary`)`` -> `null`
  [CustomLuaState]

### `Class.AudioEmitter:SetDistanceAttenuation`

``SetDistanceAttenuation(curve: `Dictionary`)`` -> `null`
  [CustomLuaState]

## Events

### `Class.AudioEmitter.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

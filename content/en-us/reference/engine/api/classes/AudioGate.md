---
title: AudioGate
type: class
superclass: Instance
---

# AudioGate

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.AudioGate.Attack` | `float` |  |
| `Class.AudioGate.Bypass` | `bool` |  |
| `Class.AudioGate.Release` | `float` |  |
| `Class.AudioGate.Threshold` | `Datatype.NumberRange` |  |

## Methods

### `Class.AudioGate:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` → `Datatype.Instances`

### `Class.AudioGate:GetInputPins`

``GetInputPins()`` → `Array`

### `Class.AudioGate:GetOutputPins`

``GetOutputPins()`` → `Array`

### `Class.AudioGate:Reset`

``Reset()`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.AudioGate.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

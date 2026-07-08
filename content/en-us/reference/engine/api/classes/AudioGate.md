---
title: AudioGate
type: class
superclass: Instance
---

# AudioGate

Mutes audio streams that fall below a certain volume threshold.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.AudioGate` behaves like a noise gate, muting audio streams when their
volume drops below a specified `Class.AudioGate.Threshold|Threshold`. It is
useful for removing background noise from microphone input or cleaning up
audio tracks. It provides one **Input** pin and one **Output** pin which can
be connected to/from by `Class.Wire|Wires`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioGate.Attack` | `float` |  |
| `Class.AudioGate.Bypass` | `bool` |  |
| `Class.AudioGate.Release` | `float` |  |
| `Class.AudioGate.Threshold` | `Datatype.NumberRange` |  |

## Methods

### `Class.AudioGate:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioGate:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.AudioGate:GetOutputPins`

``GetOutputPins()`` -> `Array`

### `Class.AudioGate:Reset`

``Reset()`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.AudioGate.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

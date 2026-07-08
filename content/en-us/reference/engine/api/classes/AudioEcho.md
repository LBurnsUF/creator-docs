---
title: AudioEcho
type: class
superclass: Instance
---

# AudioEcho

Overlays delayed copies of audio streams.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.AudioEcho` overlays delayed copies of audio streams. It provides one
**Input** pin and one **Output** pin which can be connected to/from by
`Class.Wire|Wires`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioEcho.Bypass` | `bool` |  |
| `Class.AudioEcho.DelayTime` | `float` |  |
| `Class.AudioEcho.DryLevel` | `float` |  |
| `Class.AudioEcho.Feedback` | `float` |  |
| `Class.AudioEcho.RampTime` | `float` |  |
| `Class.AudioEcho.WetLevel` | `float` |  |

## Methods

### `Class.AudioEcho:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioEcho:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.AudioEcho:GetOutputPins`

``GetOutputPins()`` -> `Array`

### `Class.AudioEcho:Reset`

``Reset()`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.AudioEcho.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

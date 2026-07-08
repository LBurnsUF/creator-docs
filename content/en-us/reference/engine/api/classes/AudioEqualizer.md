---
title: AudioEqualizer
type: class
superclass: Instance
---

# AudioEqualizer

Adjusts the frequency content of audio streams.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.AudioEqualizer` adjusts the frequency content of audio streams. It
provides one **Input** pin and one **Output** pin which can be connected
to/from by `Class.Wire|Wires`. `Class.AudioEqualizer` has 3 frequency bands
whose gain values can be controlled, and the crossover points between bands
can be moved.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioEqualizer.Bypass` | `bool` |  |
| `Class.AudioEqualizer.Editor` | `bool` | [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.AudioEqualizer.HighGain` | `float` |  |
| `Class.AudioEqualizer.LowGain` | `float` |  |
| `Class.AudioEqualizer.MidGain` | `float` |  |
| `Class.AudioEqualizer.MidRange` | `Datatype.NumberRange` |  |

## Methods

### `Class.AudioEqualizer:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioEqualizer:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.AudioEqualizer:GetOutputPins`

``GetOutputPins()`` -> `Array`

## Events

### `Class.AudioEqualizer.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

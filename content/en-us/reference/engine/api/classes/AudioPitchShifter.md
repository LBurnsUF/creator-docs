---
title: AudioPitchShifter
type: class
superclass: Instance
---

# AudioPitchShifter

Adjusts the perceived pitch of audio streams.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.AudioPitchShifter` adjusts the perceived pitch of audio streams. It
provides one **Input** pin and one **Output** pin which can be connected
to/from by `Class.Wire|Wires`. `Class.AudioPitchShifter` performs its
modifications in the frequency domain and may introduce artifacts with extreme
pitch changes.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioPitchShifter.Bypass` | `bool` |  |
| `Class.AudioPitchShifter.Pitch` | `float` |  |
| `Class.AudioPitchShifter.WindowSize` | `Enum.AudioWindowSize` |  |

## Methods

### `Class.AudioPitchShifter:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioPitchShifter:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.AudioPitchShifter:GetOutputPins`

``GetOutputPins()`` -> `Array`

## Events

### `Class.AudioPitchShifter.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

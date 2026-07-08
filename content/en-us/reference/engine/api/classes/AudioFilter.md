---
title: AudioFilter
type: class
superclass: Instance
---

# AudioFilter

Adjusts the frequency content of audio streams.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.AudioFilter` adjusts the frequency content of audio streams. It
provides one **Input** pin and one **Output** pin which can be connected
to/from by `Class.Wire|Wires`. `Class.AudioFilter` uses its
`Class.AudioFilter.FilterType|FilterType`, `Class.AudioFilter.Gain|Gain`, and
`Class.AudioFilter.Q|Q` properties to determine what to do around a particular
cutoff `Class.AudioFilter.Frequency|Frequency`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioFilter.Bypass` | `bool` |  |
| `Class.AudioFilter.Editor` | `bool` | [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.AudioFilter.FilterType` | `Enum.AudioFilterType` |  |
| `Class.AudioFilter.Frequency` | `float` |  |
| `Class.AudioFilter.Gain` | `float` |  |
| `Class.AudioFilter.Q` | `float` |  |

## Methods

### `Class.AudioFilter:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioFilter:GetGainAt`

``GetGainAt(frequency: `float`)`` -> `float`

### `Class.AudioFilter:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.AudioFilter:GetOutputPins`

``GetOutputPins()`` -> `Array`

## Events

### `Class.AudioFilter.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

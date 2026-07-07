---
title: AudioAnalyzer
type: class
superclass: Instance
---

# AudioAnalyzer

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.AudioAnalyzer.PeakLevel` | `float` | [ReadOnly] [NotReplicated] |
| `Class.AudioAnalyzer.RmsLevel` | `float` | [ReadOnly] [NotReplicated] |
| `Class.AudioAnalyzer.SpectrumEnabled` | `bool` |  |
| `Class.AudioAnalyzer.WindowSize` | `Enum.AudioWindowSize` |  |

## Methods

### `Class.AudioAnalyzer:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` → `Datatype.Instances`

### `Class.AudioAnalyzer:GetInputPins`

``GetInputPins()`` → `Array`

### `Class.AudioAnalyzer:GetOutputPins`

``GetOutputPins()`` → `Array`

### `Class.AudioAnalyzer:GetSpectrum`

``GetSpectrum()`` → `Array`
  [CustomLuaState]

## Events

### `Class.AudioAnalyzer.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

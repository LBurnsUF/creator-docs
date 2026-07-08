---
title: AudioAnalyzer
type: class
superclass: Instance
---

# AudioAnalyzer

Takes measurements from audio streams that are connected to it via one or more
`Class.Wire|Wires`.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.AudioAnalyzer` takes measurements from audio streams that are wired to
it through `Class.Wire`. It provides a single **Input** pin but does not
produce any output streams. Note that all audio processing is disabled on the
server in order to conserve resources; Properties and methods of
`Class.AudioAnalyzer` return empty or zero results when used from server
scripts.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioAnalyzer.PeakLevel` | `float` | [ReadOnly] [NotReplicated] |
| `Class.AudioAnalyzer.RmsLevel` | `float` | [ReadOnly] [NotReplicated] |
| `Class.AudioAnalyzer.SpectrumEnabled` | `bool` |  |
| `Class.AudioAnalyzer.WindowSize` | `Enum.AudioWindowSize` |  |

## Methods

### `Class.AudioAnalyzer:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioAnalyzer:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.AudioAnalyzer:GetOutputPins`

``GetOutputPins()`` -> `Array`

### `Class.AudioAnalyzer:GetSpectrum`

``GetSpectrum()`` -> `Array`
  [CustomLuaState]

## Events

### `Class.AudioAnalyzer.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

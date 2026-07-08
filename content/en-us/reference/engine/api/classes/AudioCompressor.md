---
title: AudioCompressor
type: class
superclass: Instance
---

# AudioCompressor

Adjusts the dynamic range of input streams.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.AudioCompressor` adjusts the dynamic range of audio streams. Any
momentary bursts of loudness will be clamped down according to the
compressor's properties.

`Class.AudioCompressor` provides **Input** and **Sidechain** pins that can be
targeted by `Class.Wire.TargetName`, and an **Output** pin that can be used by
`Class.Wire.SourceName`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioCompressor.Attack` | `float` |  |
| `Class.AudioCompressor.Bypass` | `bool` |  |
| `Class.AudioCompressor.Editor` | `bool` | [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.AudioCompressor.MakeupGain` | `float` |  |
| `Class.AudioCompressor.Ratio` | `float` |  |
| `Class.AudioCompressor.Release` | `float` |  |
| `Class.AudioCompressor.Threshold` | `float` |  |

## Methods

### `Class.AudioCompressor:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioCompressor:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.AudioCompressor:GetOutputPins`

``GetOutputPins()`` -> `Array`

## Events

### `Class.AudioCompressor.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

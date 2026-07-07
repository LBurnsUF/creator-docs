---
title: AudioCompressor
type: class
superclass: Instance
---

# AudioCompressor

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.AudioCompressor.Attack` | `float` |  |
| `Class.AudioCompressor.Bypass` | `bool` |  |
| `Class.AudioCompressor.Editor` | `bool` | [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.AudioCompressor.MakeupGain` | `float` |  |
| `Class.AudioCompressor.Ratio` | `float` |  |
| `Class.AudioCompressor.Release` | `float` |  |
| `Class.AudioCompressor.Threshold` | `float` |  |

## Methods

### `Class.AudioCompressor:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` → `Datatype.Instances`

### `Class.AudioCompressor:GetInputPins`

``GetInputPins()`` → `Array`

### `Class.AudioCompressor:GetOutputPins`

``GetOutputPins()`` → `Array`

## Events

### `Class.AudioCompressor.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

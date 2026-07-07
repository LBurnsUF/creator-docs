---
title: AudioEqualizer
type: class
superclass: Instance
---

# AudioEqualizer

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.AudioEqualizer.Bypass` | `bool` |  |
| `Class.AudioEqualizer.Editor` | `bool` | [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.AudioEqualizer.HighGain` | `float` |  |
| `Class.AudioEqualizer.LowGain` | `float` |  |
| `Class.AudioEqualizer.MidGain` | `float` |  |
| `Class.AudioEqualizer.MidRange` | `Datatype.NumberRange` |  |

## Methods

### `Class.AudioEqualizer:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` → `Datatype.Instances`

### `Class.AudioEqualizer:GetInputPins`

``GetInputPins()`` → `Array`

### `Class.AudioEqualizer:GetOutputPins`

``GetOutputPins()`` → `Array`

## Events

### `Class.AudioEqualizer.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

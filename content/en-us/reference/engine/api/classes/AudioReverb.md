---
title: AudioReverb
type: class
superclass: Instance
---

# AudioReverb

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.AudioReverb.Bypass` | `bool` |  |
| `Class.AudioReverb.DecayRatio` | `float` |  |
| `Class.AudioReverb.DecayTime` | `float` |  |
| `Class.AudioReverb.Density` | `float` |  |
| `Class.AudioReverb.Diffusion` | `float` |  |
| `Class.AudioReverb.DryLevel` | `float` |  |
| `Class.AudioReverb.EarlyDelayTime` | `float` |  |
| `Class.AudioReverb.HighCutFrequency` | `float` |  |
| `Class.AudioReverb.LateDelayTime` | `float` |  |
| `Class.AudioReverb.LowShelfFrequency` | `float` |  |
| `Class.AudioReverb.LowShelfGain` | `float` |  |
| `Class.AudioReverb.ReferenceFrequency` | `float` |  |
| `Class.AudioReverb.WetLevel` | `float` |  |

## Methods

### `Class.AudioReverb:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` → `Datatype.Instances`

### `Class.AudioReverb:GetInputPins`

``GetInputPins()`` → `Array`

### `Class.AudioReverb:GetOutputPins`

``GetOutputPins()`` → `Array`

### `Class.AudioReverb:Reset`

``Reset()`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.AudioReverb.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

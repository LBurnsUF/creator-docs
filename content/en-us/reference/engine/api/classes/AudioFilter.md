---
title: AudioFilter
type: class
superclass: Instance
---

# AudioFilter

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.AudioFilter.Bypass` | `bool` |  |
| `Class.AudioFilter.Editor` | `bool` | [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.AudioFilter.FilterType` | `Enum.AudioFilterType` |  |
| `Class.AudioFilter.Frequency` | `float` |  |
| `Class.AudioFilter.Gain` | `float` |  |
| `Class.AudioFilter.Q` | `float` |  |

## Methods

### `Class.AudioFilter:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` → `Datatype.Instances`

### `Class.AudioFilter:GetGainAt`

``GetGainAt(frequency: `float`)`` → `float`

### `Class.AudioFilter:GetInputPins`

``GetInputPins()`` → `Array`

### `Class.AudioFilter:GetOutputPins`

``GetOutputPins()`` → `Array`

## Events

### `Class.AudioFilter.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

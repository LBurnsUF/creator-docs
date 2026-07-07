---
title: AudioFlanger
type: class
superclass: Instance
---

# AudioFlanger

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.AudioFlanger.Bypass` | `bool` |  |
| `Class.AudioFlanger.Depth` | `float` |  |
| `Class.AudioFlanger.Mix` | `float` |  |
| `Class.AudioFlanger.Rate` | `float` |  |

## Methods

### `Class.AudioFlanger:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` → `Datatype.Instances`

### `Class.AudioFlanger:GetInputPins`

``GetInputPins()`` → `Array`

### `Class.AudioFlanger:GetOutputPins`

``GetOutputPins()`` → `Array`

## Events

### `Class.AudioFlanger.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

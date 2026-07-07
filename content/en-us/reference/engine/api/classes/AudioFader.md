---
title: AudioFader
type: class
superclass: Instance
---

# AudioFader

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.AudioFader.Bypass` | `bool` |  |
| `Class.AudioFader.Volume` | `float` |  |

## Methods

### `Class.AudioFader:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` → `Datatype.Instances`

### `Class.AudioFader:GetInputPins`

``GetInputPins()`` → `Array`

### `Class.AudioFader:GetOutputPins`

``GetOutputPins()`` → `Array`

## Events

### `Class.AudioFader.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

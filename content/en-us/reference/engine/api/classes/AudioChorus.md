---
title: AudioChorus
type: class
superclass: Instance
---

# AudioChorus

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.AudioChorus.Bypass` | `bool` |  |
| `Class.AudioChorus.Depth` | `float` |  |
| `Class.AudioChorus.Mix` | `float` |  |
| `Class.AudioChorus.Rate` | `float` |  |

## Methods

### `Class.AudioChorus:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` → `Datatype.Instances`

### `Class.AudioChorus:GetInputPins`

``GetInputPins()`` → `Array`

### `Class.AudioChorus:GetOutputPins`

``GetOutputPins()`` → `Array`

## Events

### `Class.AudioChorus.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

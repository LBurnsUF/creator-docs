---
title: AudioDistortion
type: class
superclass: Instance
---

# AudioDistortion

Distorts audio streams, making them sound fuzzier, grittier, and louder.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.AudioDistortion` distorts audio streams, making them sound fuzzier,
grittier, and louder. It provides one **Input** pin and one **Output** pin
which can be connected to/from by `Class.Wire|Wires`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioDistortion.Bypass` | `bool` |  |
| `Class.AudioDistortion.Level` | `float` |  |

## Methods

### `Class.AudioDistortion:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioDistortion:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.AudioDistortion:GetOutputPins`

``GetOutputPins()`` -> `Array`

## Events

### `Class.AudioDistortion.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

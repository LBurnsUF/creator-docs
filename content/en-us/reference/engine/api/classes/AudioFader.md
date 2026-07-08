---
title: AudioFader
type: class
superclass: Instance
---

# AudioFader

Adjusts the volume of audio streams.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.AudioFader` adjusts the volume of audio streams. It provides one
**Input** pin and one **Output** pin which can be connected to/from by
`Class.Wire|Wires`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioFader.Bypass` | `bool` |  |
| `Class.AudioFader.Volume` | `float` |  |

## Methods

### `Class.AudioFader:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioFader:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.AudioFader:GetOutputPins`

``GetOutputPins()`` -> `Array`

## Events

### `Class.AudioFader.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

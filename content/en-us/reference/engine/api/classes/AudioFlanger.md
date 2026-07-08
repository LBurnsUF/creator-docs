---
title: AudioFlanger
type: class
superclass: Instance
---

# AudioFlanger

Imparts a whooshing or sweeping sound on audio streams.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.AudioFlanger` imparts a whooshing or sweeping sound on audio streams by
overlaying a delayed copy of the input stream and modulating the pitch of the
copy. It provides one **Input** pin and one **Output** pin which can be
connected to/from by `Class.Wire|Wires`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioFlanger.Bypass` | `bool` |  |
| `Class.AudioFlanger.Depth` | `float` |  |
| `Class.AudioFlanger.Mix` | `float` |  |
| `Class.AudioFlanger.Rate` | `float` |  |

## Methods

### `Class.AudioFlanger:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioFlanger:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.AudioFlanger:GetOutputPins`

``GetOutputPins()`` -> `Array`

## Events

### `Class.AudioFlanger.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

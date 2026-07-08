---
title: AudioChorus
type: class
superclass: Instance
---

# AudioChorus

Makes an audio stream sound more voluminous. If applied to a single voice, it
may sound like multiple voices.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.AudioChorus` makes an audio stream sound more voluminous. It provides
one **Input** pin and one **Output** pin which can be connected to/from by
`Class.Wire|Wires`.

`Class.AudioChorus` is implemented by duplicating the input stream and
modulating the pitch of several delayed copies so that the overall result
sounds like a cloud of streams. If applied to a single voice, it may sound
like multiple voices.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioChorus.Bypass` | `bool` |  |
| `Class.AudioChorus.Depth` | `float` |  |
| `Class.AudioChorus.Mix` | `float` |  |
| `Class.AudioChorus.Rate` | `float` |  |

## Methods

### `Class.AudioChorus:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioChorus:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.AudioChorus:GetOutputPins`

``GetOutputPins()`` -> `Array`

## Events

### `Class.AudioChorus.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

---
title: AudioTremolo
type: class
superclass: Instance
---

# AudioTremolo

Creates a trembling effect on a sound by varying the volume of the sound up
and down.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.AudioTremolo` creates a trembling effect on a sound by varying the
volume of the sound up and down. It provides one **Input** pin and one
**Output** pin which can be connected to/from by `Class.Wire|Wires`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioTremolo.Bypass` | `bool` |  |
| `Class.AudioTremolo.Depth` | `float` |  |
| `Class.AudioTremolo.Duty` | `float` |  |
| `Class.AudioTremolo.Frequency` | `float` |  |
| `Class.AudioTremolo.Shape` | `float` |  |
| `Class.AudioTremolo.Skew` | `float` |  |
| `Class.AudioTremolo.Square` | `float` |  |

## Methods

### `Class.AudioTremolo:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioTremolo:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.AudioTremolo:GetOutputPins`

``GetOutputPins()`` -> `Array`

## Events

### `Class.AudioTremolo.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

---
title: AudioChannelSplitter
type: class
superclass: Instance
---

# AudioChannelSplitter

Splits an audio stream into component channels so that each can be processed
independently.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.AudioChannelSplitter` splits an audio stream into component channels so
that each can be processed independently. It provides one **Input** pin, one
combined **Output** pin, as well as the following secondary output pins, all
of which can be connected to/from by `Class.Wire|Wires`: **Left**, **Right**,
**Center**, **SurroundLeft**, **SurroundRight**, **Sub**, **BackLeft**,
**BackRight**, **TopLeft**, **TopRight**, **TopBackLeft**, and
**TopBackRight**.

<img src="/assets/engine-api/enums/AudioChannelLayout/Surround_7_1_4.jpg" width="810" alt="Diagram showing position of all potential channels." />

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioChannelSplitter.Layout` | `Enum.AudioChannelLayout` |  |

## Methods

### `Class.AudioChannelSplitter:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioChannelSplitter:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.AudioChannelSplitter:GetOutputPins`

``GetOutputPins()`` -> `Array`

## Events

### `Class.AudioChannelSplitter.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

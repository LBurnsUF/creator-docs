---
title: AudioChannelMixer
type: class
superclass: Instance
---

# AudioChannelMixer

Combines multiple audio streams into a single, multichannel audio stream.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.AudioChannelMixer` mixes multiple audio streams into a single,
multichannel stream. It provides one combined **Input** pin, one **Output**
pin, as well as the following secondary input pins, all of which can be
connected to/from by `Class.Wire|Wires`: **Left**, **Right**, **Center**,
**SurroundLeft**, **SurroundRight**, **Sub**, **BackLeft**, **BackRight**,
**TopLeft**, **TopRight**, **TopBackLeft**, and **TopBackRight**.

<img src="/assets/engine-api/enums/AudioChannelLayout/Surround_7_1_4.jpg" width="810" alt="Diagram showing position of all potential channels." />

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioChannelMixer.Layout` | `Enum.AudioChannelLayout` |  |

## Methods

### `Class.AudioChannelMixer:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioChannelMixer:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.AudioChannelMixer:GetOutputPins`

``GetOutputPins()`` -> `Array`

## Events

### `Class.AudioChannelMixer.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

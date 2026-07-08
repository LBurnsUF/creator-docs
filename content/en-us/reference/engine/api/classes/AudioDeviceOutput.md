---
title: AudioDeviceOutput
type: class
superclass: Instance
---

# AudioDeviceOutput

Accepts audio streams to be rendered out to physical hardware devices such as
speakers or headphones.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.AudioDeviceOutput` accepts audio streams to be rendered out to physical
hardware devices such as speakers or headphones. It provides a single
**Input** pin that can be targeted by `Class.Wire|Wires`. Any audio streams
wired to an `Class.AudioDeviceOutput` are heard.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioDeviceOutput.Player` | `Class.Player` |  |

## Methods

### `Class.AudioDeviceOutput:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioDeviceOutput:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.AudioDeviceOutput:GetOutputPins`

``GetOutputPins()`` -> `Array`

## Events

### `Class.AudioDeviceOutput.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

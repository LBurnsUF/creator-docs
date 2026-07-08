---
title: AudioLimiter
type: class
superclass: Instance
---

# AudioLimiter

Limits how loud audio streams are allowed to be.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`AudioLimiter` limits how loud audio streams are allowed to be. Whenever its
input stream exceeds a specified maximum level, the stream's volume is reduced
for a moment. `AudioLimiter` provides a single **Input** pin, and a single
**Output** pin that can be connected to/from by `Class.Wires`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioLimiter.Bypass` | `bool` |  |
| `Class.AudioLimiter.Editor` | `bool` | [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.AudioLimiter.MaxLevel` | `float` |  |
| `Class.AudioLimiter.Release` | `float` |  |

## Methods

### `Class.AudioLimiter:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioLimiter:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.AudioLimiter:GetOutputPins`

``GetOutputPins()`` -> `Array`

## Events

### `Class.AudioLimiter.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

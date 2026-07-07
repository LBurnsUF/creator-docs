---
title: AudioEcho
type: class
superclass: Instance
---

# AudioEcho

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.AudioEcho.Bypass` | `bool` |  |
| `Class.AudioEcho.DelayTime` | `float` |  |
| `Class.AudioEcho.DryLevel` | `float` |  |
| `Class.AudioEcho.Feedback` | `float` |  |
| `Class.AudioEcho.RampTime` | `float` |  |
| `Class.AudioEcho.WetLevel` | `float` |  |

## Methods

### `Class.AudioEcho:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` → `Datatype.Instances`

### `Class.AudioEcho:GetInputPins`

``GetInputPins()`` → `Array`

### `Class.AudioEcho:GetOutputPins`

``GetOutputPins()`` → `Array`

### `Class.AudioEcho:Reset`

``Reset()`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.AudioEcho.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

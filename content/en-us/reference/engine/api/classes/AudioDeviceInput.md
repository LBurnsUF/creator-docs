---
title: AudioDeviceInput
type: class
superclass: Instance
---

# AudioDeviceInput

Produces audio streams from physical devices, such as microphones.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.AudioDeviceInput` produces audio streams from physical devices, such as
microphones. It provides a single **Output** pin which can be connected to
other pins via `Class.Wire|Wires`. `Class.AudioDeviceInput` has properties for
selecting which `Class.Player` is producing the stream, and controlling
whether or not they are muted.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioDeviceInput.AccessType` | `Enum.AccessModifierType` |  |
| `Class.AudioDeviceInput.Active` | `bool` |  {write: RobloxScriptSecurity} |
| `Class.AudioDeviceInput.EchoCancellation` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.AudioDeviceInput.GainControl` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.AudioDeviceInput.IsReady` | `bool` | [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.AudioDeviceInput.Muted` | `bool` |  |
| `Class.AudioDeviceInput.MutedByLocalUser` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.AudioDeviceInput.NoiseSuppression` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.AudioDeviceInput.Player` | `Class.Player` |  |
| `Class.AudioDeviceInput.Volume` | `float` |  |

## Methods

### `Class.AudioDeviceInput:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioDeviceInput:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.AudioDeviceInput:GetOutputPins`

``GetOutputPins()`` -> `Array`

### `Class.AudioDeviceInput:GetUserIdAccessList`

``GetUserIdAccessList()`` -> `Array`

### `Class.AudioDeviceInput:SetUserIdAccessList`

``SetUserIdAccessList(userIds: `Array`)`` -> `null`

## Events

### `Class.AudioDeviceInput.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

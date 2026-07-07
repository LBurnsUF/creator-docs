---
title: RealtimeMedia
type: class
superclass: Instance
---

# RealtimeMedia

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.RealtimeMedia.ForwardInput` | `bool` |  {security: RobloxScriptSecurity} |
| `Class.RealtimeMedia.IsConnected` | `bool` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.RealtimeMedia:ConnectAsync`

``ConnectAsync(serverUrl: `string`, connectParams: `Dictionary`)`` → `bool`
  [Yields]

### `Class.RealtimeMedia:Disconnect`

``Disconnect()`` → `null`

### `Class.RealtimeMedia:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` → `Datatype.Instances`

### `Class.RealtimeMedia:GetInputPins`

``GetInputPins()`` → `Array`

### `Class.RealtimeMedia:GetOutputPins`

``GetOutputPins()`` → `Array`

### `Class.RealtimeMedia:SendMessage`

``SendMessage(message: `string`, binary: `bool`)`` → `bool`

## Events

### `Class.RealtimeMedia.OnMessage`

Fires with: (message: `string`, binary: `bool`)

### `Class.RealtimeMedia.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)

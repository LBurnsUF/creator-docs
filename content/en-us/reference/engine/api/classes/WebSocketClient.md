---
title: WebSocketClient
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# WebSocketClient

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.WebSocketClient.ConnectionState` | `Enum.WebSocketState` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.WebSocketClient:Close`

``Close()`` → `null`

### `Class.WebSocketClient:Send`

``Send(data: `string`)`` → `null`

## Events

### `Class.WebSocketClient.Closed`

Fires with: ()

### `Class.WebSocketClient.MessageReceived`

Fires with: (data: `string`)

### `Class.WebSocketClient.Opened`

Fires with: ()

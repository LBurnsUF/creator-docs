---
title: WebStreamClient
type: class
superclass: Object
tags: [NotCreatable, NotReplicated]
---

# WebStreamClient

Maintains a streaming connection.

**Inherits from:** `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

Maintains a streaming connection. To process stream events as they arrive,
connect callback functions to each event using
`Datatype.RBXScriptSignal:Connect()`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.WebStreamClient.ConnectionState` | `Enum.WebStreamClientState` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.WebStreamClient:Close`

``Close()`` -> `null`

### `Class.WebStreamClient:Send`

``Send(data: `string`)`` -> `null`

## Events

### `Class.WebStreamClient.Closed`

Fires with: ()

### `Class.WebStreamClient.Error`

Fires with: (responseStatusCode: `int`, errorMessage: `string`)

### `Class.WebStreamClient.MessageReceived`

Fires with: (message: `string`)

### `Class.WebStreamClient.Opened`

Fires with: (responseStatusCode: `int`, headers: `string`)

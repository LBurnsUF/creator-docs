---
title: PluginConnection
type: class
superclass: Object
tags: [NotCreatable, NotReplicated]
---

# PluginConnection

Encapsulates a connection between the current data model and another for
plugin communication.

**Inherits from:** `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

Studio plugins run in each Studio data model that the user opens, including
both edit and playtest data models. `PluginConnection` objects allow these
instances of the same plugin to communicate across data model boundaries.
Messages sent by `Class.PluginConnection:SendMessage()` will be received in
the remote data model via the callback the same plugin registers with
`Class.PluginConnection:BindToMessage()`. Each `PluginConnection` object can
both send and receive messages while connected, and messages will be received
reliably and in order unless the connection drops (e.g. due to the remote data
model shutting down) before their receipt.

Note that although multiple plugins may share the same `PluginConnection`
object, they each have their own internal connection; each plugin will receive
only its own messages in its callback to `BindToMessage()`, even if other
plugins call `SendMessage()`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.PluginConnection.Connected` | `bool` | [ReadOnly] [NotReplicated] {security: PluginSecurity} |
| `Class.PluginConnection.TargetId` | `string` | [ReadOnly] [NotReplicated] {security: PluginSecurity} |
| `Class.PluginConnection.Type` | `Enum.PluginConnectionTargetType` | [ReadOnly] [NotReplicated] {security: PluginSecurity} |

## Methods

### `Class.PluginConnection:BindToMessage`

``BindToMessage(callbackFunction: `Datatype.Function`)`` -> `Datatype.RBXScriptConnection`
   {security: PluginSecurity}

### `Class.PluginConnection:SendMessage`

``SendMessage(message: `Variant`)`` -> `null`
   {security: PluginSecurity}

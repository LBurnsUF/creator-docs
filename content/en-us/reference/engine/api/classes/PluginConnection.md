---
title: PluginConnection
type: class
superclass: Object
tags: [NotCreatable, NotReplicated]
---

# PluginConnection

**Inherits from:** `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.PluginConnection.Connected` | `bool` | [ReadOnly] [NotReplicated] {security: PluginSecurity} |
| `Class.PluginConnection.TargetId` | `string` | [ReadOnly] [NotReplicated] {security: PluginSecurity} |
| `Class.PluginConnection.Type` | `Enum.PluginConnectionTargetType` | [ReadOnly] [NotReplicated] {security: PluginSecurity} |

## Methods

### `Class.PluginConnection:BindToMessage`

``BindToMessage(callbackFunction: `Datatype.Function`)`` → `Datatype.RBXScriptConnection`
   {security: PluginSecurity}

### `Class.PluginConnection:SendMessage`

``SendMessage(message: `Variant`)`` → `null`
   {security: PluginSecurity}

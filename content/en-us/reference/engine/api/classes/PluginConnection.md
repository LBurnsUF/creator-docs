---
title: PluginConnection
type: class
superclass: Object
tags: [NotCreatable, NotReplicated]
---

# PluginConnection

**Inherits**: Object

**Tags**: NotCreatable, NotReplicated

## Properties

- **Connected**: `bool` [ReadOnly] [NotReplicated] (Security: Read=PluginSecurity, Write=PluginSecurity)
- **TargetId**: `string` [ReadOnly] [NotReplicated] (Security: Read=PluginSecurity, Write=PluginSecurity)
- **Type**: `PluginConnectionTargetType` [ReadOnly] [NotReplicated] (Security: Read=PluginSecurity, Write=PluginSecurity)

## Methods

- **BindToMessage**(`callbackFunction: Function`) -> `RBXScriptConnection`
- **SendMessage**(`message: Variant`) -> `null`

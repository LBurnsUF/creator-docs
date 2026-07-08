---
title: DebuggerConnectionManager
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# DebuggerConnectionManager

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.DebuggerConnectionManager.Timeout` | `double` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |

## Methods

### `Class.DebuggerConnectionManager:ConnectLocal`

``ConnectLocal(dataModel: `Class.DataModel`)`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.DebuggerConnectionManager:FocusConnection`

``FocusConnection(connection: `Class.DebuggerConnection`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.DebuggerConnectionManager:GetAvailableConnection`

``GetAvailableConnection()`` -> `Class.DebuggerConnection`
   {security: RobloxScriptSecurity}

### `Class.DebuggerConnectionManager:GetConnectionById`

``GetConnectionById(id: `int`)`` -> `Class.DebuggerConnection`
   {security: RobloxScriptSecurity}

## Events

### `Class.DebuggerConnectionManager.ConnectionEnded`

Fires with: (connection: `Class.DebuggerConnection`, reason: `Enum.DebuggerEndReason`)

### `Class.DebuggerConnectionManager.ConnectionStarted`

Fires with: (connection: `Class.DebuggerConnection`)

### `Class.DebuggerConnectionManager.FocusChanged`

Fires with: (connection: `Class.DebuggerConnection`)

---
title: DebuggerManager
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# DebuggerManager

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.DebuggerManager.DebuggingEnabled` | `bool` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.DebuggerManager:AddDebugger`

``AddDebugger(script: `Class.Instance`)`` -> `Class.Instance`

### `Class.DebuggerManager:EnableDebugging`

``EnableDebugging()`` -> `null`
   {security: LocalUserSecurity}

### `Class.DebuggerManager:GetDebuggers`

``GetDebuggers()`` -> `Datatype.Instances`

### `Class.DebuggerManager:Resume`

``Resume()`` -> `null`

### `Class.DebuggerManager:StepIn`

``StepIn()`` -> `null`
  [Deprecated]

### `Class.DebuggerManager:StepOut`

``StepOut()`` -> `null`
  [Deprecated]

### `Class.DebuggerManager:StepOver`

``StepOver()`` -> `null`
  [Deprecated]

## Events

### `Class.DebuggerManager.DebuggerAdded`

Fires with: (debugger: `Class.Instance`)

### `Class.DebuggerManager.DebuggerRemoved`

Fires with: (debugger: `Class.Instance`)

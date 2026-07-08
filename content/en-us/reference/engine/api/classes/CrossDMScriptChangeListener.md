---
title: CrossDMScriptChangeListener
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# CrossDMScriptChangeListener

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.CrossDMScriptChangeListener:IsWatchingScriptLine`

``IsWatchingScriptLine(scriptRef: `string`, lineNumber: `int`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.CrossDMScriptChangeListener:StartWatchingScriptLine`

``StartWatchingScriptLine(scriptRef: `string`, debuggerConnectionId: `int`, lineNumber: `int`)`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.CrossDMScriptChangeListener.GuidLineContentsChanged`

Fires with: (guid: `string`, lineNumber: `int`, contents: `string`)

### `Class.CrossDMScriptChangeListener.GuidNameChanged`

Fires with: (guid: `string`, fullName: `string`)

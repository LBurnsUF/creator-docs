---
title: CrossDMScriptChangeListener
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# CrossDMScriptChangeListener

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **IsWatchingScriptLine**(`scriptRef: string`, `lineNumber: int`) -> `bool`
- **StartWatchingScriptLine**(`scriptRef: string`, `debuggerConnectionId: int`, `lineNumber: int`) -> `null`

## Events

- **GuidLineContentsChanged**(`guid: string`, `lineNumber: int`, `contents: string`)
- **GuidNameChanged**(`guid: string`, `fullName: string`)

---
title: ScriptContext
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ScriptContext

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **ScriptsDisabled**: `bool` [Hidden] (Security: Read=LocalUserSecurity, Write=LocalUserSecurity)

## Methods

- **AddCoreScriptLocal**(`name: string`, `parent: Instance`) -> `null`
- **CompressLuaApp**() -> `null`
- **EnableCoverage**(`instance: Instance`) -> `null`
- **GetCoverageStats**() -> `Array`
- **GetLuauHeapInstanceReferenceReport**(`target: string`) -> `Dictionary` [CustomLuaState]
- **GetLuauHeapMemoryReport**(`target: string`) -> `Dictionary` [CustomLuaState]
- **ReportLuaRequireCount**() -> `null`
- **SetTimeout**(`seconds: double`) -> `null`

## Events

- **Error**(`message: string`, `stackTrace: string`, `script: Instance`)
- **ErrorDetailed**(`message: string`, `stackTrace: string`, `script: Instance`, `details: string`, `securityLevel: int`, `messageId: string`)

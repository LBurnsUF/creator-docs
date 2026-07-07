---
title: MicroProfilerService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# MicroProfilerService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **ContextLabel**: `string` (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **DumpToFileAsync**(`secondsToDelay: int`, `framesToDump: int`) -> `string` [Yields]
- **GetDataInRange**(`slotId: int`, `offset: int`, `size: int`, `destBuffer: buffer`, `destBufferOffset: int`) -> `int` [CustomLuaState]
- **GetDataSize**(`slotId: int`) -> `int`
- **ProcessCommand**(`cmdBuf: buffer`, `cmdOffset: int`, `cmdSize: int`, `respBuf: buffer`, `respOffset: int`, `respSize: int`) -> `int` [CustomLuaState]

## Events

- **DataChanged**(`slotId: int`, `flags: int`)

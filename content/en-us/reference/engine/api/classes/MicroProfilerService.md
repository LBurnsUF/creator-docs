---
title: MicroProfilerService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# MicroProfilerService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.MicroProfilerService.ContextLabel` | `string` |  {security: RobloxScriptSecurity} |

## Methods

### `Class.MicroProfilerService:DumpToFileAsync`

``DumpToFileAsync(secondsToDelay: `int`, framesToDump: `int`)`` → `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.MicroProfilerService:GetDataInRange`

``GetDataInRange(slotId: `int`, offset: `int`, size: `int`, destBuffer: `Datatype.buffer`, destBufferOffset: `int`)`` → `int`
  [CustomLuaState]

### `Class.MicroProfilerService:GetDataSize`

``GetDataSize(slotId: `int`)`` → `int`

### `Class.MicroProfilerService:ProcessCommand`

``ProcessCommand(cmdBuf: `Datatype.buffer`, cmdOffset: `int`, cmdSize: `int`, respBuf: `Datatype.buffer`, respOffset: `int`, respSize: `int`)`` → `int`
  [CustomLuaState]

## Events

### `Class.MicroProfilerService.DataChanged`

Fires with: (slotId: `int`, flags: `int`)

---
title: HeapProfilerService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# HeapProfilerService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.HeapProfilerService:ClientRequestDataAsync`

``ClientRequestDataAsync(player: `Class.Player`)`` → `string`
  [Yields] {security: PluginSecurity}

### `Class.HeapProfilerService:ServerRequestDataAsync`

``ServerRequestDataAsync()`` → `string`
  [Yields] {security: PluginSecurity}

## Events

### `Class.HeapProfilerService.OnNewData`

Fires with: (player: `Class.Player`, jsonString: `Datatype.buffer`, id: `int`, compressedLength: `int`, uncompressedLength: `int`)

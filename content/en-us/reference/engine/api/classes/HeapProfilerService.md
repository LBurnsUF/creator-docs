---
title: HeapProfilerService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# HeapProfilerService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **ClientRequestDataAsync**(`player: Player`) -> `string` [Yields]
- **ServerRequestDataAsync**() -> `string` [Yields]

## Events

- **OnNewData**(`player: Player`, `jsonString: buffer`, `id: int`, `compressedLength: int`, `uncompressedLength: int`)

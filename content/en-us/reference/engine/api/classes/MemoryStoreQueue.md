---
title: MemoryStoreQueue
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# MemoryStoreQueue

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Methods

### `Class.MemoryStoreQueue:AddAsync`

``AddAsync(value: `Variant`, expiration: `int64`, priority: `double`)`` → `null`
  [Yields]

### `Class.MemoryStoreQueue:GetSizeAsync`

``GetSizeAsync(excludeInvisible: `bool`)`` → `int`
  [Yields]

### `Class.MemoryStoreQueue:ReadAsync`

``ReadAsync(count: `int`, allOrNothing: `bool`, waitTimeout: `double`)`` → `Tuple`
  [Yields]

### `Class.MemoryStoreQueue:RemoveAsync`

``RemoveAsync(id: `string`)`` → `null`
  [Yields]

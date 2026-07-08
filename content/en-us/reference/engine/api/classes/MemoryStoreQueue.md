---
title: MemoryStoreQueue
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# MemoryStoreQueue

Provides access to a queue within MemoryStore.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

Provides access to a queue within MemoryStore. A queue is a data structure
that provides temporary storage for arbitrary items (up to the maximum item
size -- see
[MemoryStore Limits](../../../cloud-services/memory-stores/index.md#limits-and-quotas)).
Each queue item has a numeric priority: MemoryStore retrieves items with
higher priority from the queue first, and it retrieves Items with the same
priority in order of addition.

Items in the queue can optionally be set to expire after a certain amount of
time. Expired items simply disappear from the queue as if they were never
added.

## Methods

### `Class.MemoryStoreQueue:AddAsync`

``AddAsync(value: `Variant`, expiration: `int64`, priority: `double`)`` -> `null`
  [Yields]

### `Class.MemoryStoreQueue:GetSizeAsync`

``GetSizeAsync(excludeInvisible: `bool`)`` -> `int`
  [Yields]

### `Class.MemoryStoreQueue:ReadAsync`

``ReadAsync(count: `int`, allOrNothing: `bool`, waitTimeout: `double`)`` -> `Tuple`
  [Yields]

### `Class.MemoryStoreQueue:RemoveAsync`

``RemoveAsync(id: `string`)`` -> `null`
  [Yields]

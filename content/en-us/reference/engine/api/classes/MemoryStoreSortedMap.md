---
title: MemoryStoreSortedMap
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# MemoryStoreSortedMap

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Methods

### `Class.MemoryStoreSortedMap:GetAsync`

``GetAsync(key: `string`)`` → `Tuple`
  [Yields]

### `Class.MemoryStoreSortedMap:GetRangeAsync`

``GetRangeAsync(direction: `Enum.SortDirection`, count: `int`, exclusiveLowerBound: `Variant`, exclusiveUpperBound: `Variant`)`` → `Array`
  [Yields]

### `Class.MemoryStoreSortedMap:GetSizeAsync`

``GetSizeAsync()`` → `int`
  [Yields]

### `Class.MemoryStoreSortedMap:RemoveAsync`

``RemoveAsync(key: `string`)`` → `null`
  [Yields]

### `Class.MemoryStoreSortedMap:SetAsync`

``SetAsync(key: `string`, value: `Variant`, expiration: `int64`, sortKey: `Variant`)`` → `bool`
  [Yields]

### `Class.MemoryStoreSortedMap:UpdateAsync`

``UpdateAsync(key: `string`, transformFunction: `Datatype.Function`, expiration: `int64`)`` → `Tuple`
  [Yields]

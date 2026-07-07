---
title: MemoryStoreHashMap
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# MemoryStoreHashMap

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Methods

### `Class.MemoryStoreHashMap:GetAsync`

``GetAsync(key: `string`)`` → `Variant`
  [Yields]

### `Class.MemoryStoreHashMap:ListItemsAsync`

``ListItemsAsync(count: `int`)`` → `Class.MemoryStoreHashMapPages`
  [Yields]

### `Class.MemoryStoreHashMap:RemoveAsync`

``RemoveAsync(key: `string`)`` → `null`
  [Yields]

### `Class.MemoryStoreHashMap:SetAsync`

``SetAsync(key: `string`, value: `Variant`, expiration: `int64`)`` → `bool`
  [Yields]

### `Class.MemoryStoreHashMap:UpdateAsync`

``UpdateAsync(key: `string`, transformFunction: `Datatype.Function`, expiration: `int64`)`` → `Variant`
  [Yields]

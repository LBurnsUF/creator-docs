---
title: MemoryStoreHashMap
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# MemoryStoreHashMap

Provides access to a hash map within `Class.MemoryStoreService`.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

Provides access to a hash map within `Class.MemoryStoreService`. A hash map is
a collection of items where string keys are associated with arbitrary values
(up to the maximum allowed size -- see
[Memory Stores](../../../cloud-services/memory-stores/hash-map.md)). The keys
have no ordering guarantees.

## Methods

### `Class.MemoryStoreHashMap:GetAsync`

``GetAsync(key: `string`)`` -> `Variant`
  [Yields]

### `Class.MemoryStoreHashMap:ListItemsAsync`

``ListItemsAsync(count: `int`)`` -> `Class.MemoryStoreHashMapPages`
  [Yields]

### `Class.MemoryStoreHashMap:RemoveAsync`

``RemoveAsync(key: `string`)`` -> `null`
  [Yields]

### `Class.MemoryStoreHashMap:SetAsync`

``SetAsync(key: `string`, value: `Variant`, expiration: `int64`)`` -> `bool`
  [Yields]

### `Class.MemoryStoreHashMap:UpdateAsync`

``UpdateAsync(key: `string`, transformFunction: `Datatype.Function`, expiration: `int64`)`` -> `Variant`
  [Yields]

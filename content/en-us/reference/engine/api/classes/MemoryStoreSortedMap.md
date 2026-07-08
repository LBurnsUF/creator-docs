---
title: MemoryStoreSortedMap
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# MemoryStoreSortedMap

Provides access to a sorted map within `Class.MemoryStoreService`.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

Provides access to a sorted map within `Class.MemoryStoreService`. A sorted
map is a collection of items where string keys are associated with arbitrary
values (up to the maximum allowed size -- see
[Memory Stores](../../../cloud-services/memory-stores/sorted-map.md)). Each
item can also have an optional sort key, which can be a number or a string. In
the ordering of items, the sort key, if provided, takes precedence over the
key. Items with numeric sort keys are sorted before items with string sort
keys, which are sorted before items with no sort key. Items with the same sort
key and items with no sort key are arranged in alphabetical order by key.

## Methods

### `Class.MemoryStoreSortedMap:GetAsync`

``GetAsync(key: `string`)`` -> `Tuple`
  [Yields]

### `Class.MemoryStoreSortedMap:GetRangeAsync`

``GetRangeAsync(direction: `Enum.SortDirection`, count: `int`, exclusiveLowerBound: `Variant`, exclusiveUpperBound: `Variant`)`` -> `Array`
  [Yields]

### `Class.MemoryStoreSortedMap:GetSizeAsync`

``GetSizeAsync()`` -> `int`
  [Yields]

### `Class.MemoryStoreSortedMap:RemoveAsync`

``RemoveAsync(key: `string`)`` -> `null`
  [Yields]

### `Class.MemoryStoreSortedMap:SetAsync`

``SetAsync(key: `string`, value: `Variant`, expiration: `int64`, sortKey: `Variant`)`` -> `bool`
  [Yields]

### `Class.MemoryStoreSortedMap:UpdateAsync`

``UpdateAsync(key: `string`, transformFunction: `Datatype.Function`, expiration: `int64`)`` -> `Tuple`
  [Yields]

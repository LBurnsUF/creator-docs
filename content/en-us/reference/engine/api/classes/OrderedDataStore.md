---
title: OrderedDataStore
type: class
superclass: GlobalDataStore
tags: [NotCreatable, NotReplicated]
---

# OrderedDataStore

A GlobalDataStore that also allows for ordered data store entries.

**Inherits from:** `Class.GlobalDataStore` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

A **OrderedDataStore** is essentially a `Class.GlobalDataStore` with the
exception that stored values must be **integers**. It exposes a method
`Class.OrderedDataStore:GetSortedAsync()|GetSortedAsync()` which allows
inspection of the entries in sorted order using a `Class.DataStorePages`
object.

Ordered data stores do not support versioning and metadata, so
`Class.DataStoreKeyInfo` is always `nil` for keys in an
`Class.OrderedDataStore`. If you need versioning and metadata support, use a
`Class.DataStore`.

Ordered data stores do not support the optional `userIds` parameter for
`Class.OrderedDataStore:SetAsync()|SetAsync()` or
`Class.OrderedDataStore:IncrementAsync()|IncrementAsync()`.

See [Data stores](../../../cloud-services/data-stores/index.md) for an
overview on how to use ordered data stores.

## Methods

### `Class.OrderedDataStore:GetSortedAsync`

``GetSortedAsync(ascending: `bool`, pagesize: `int`, minValue: `Variant`, maxValue: `Variant`)`` -> `Class.DataStorePages`
  [Yields]

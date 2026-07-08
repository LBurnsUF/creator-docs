---
title: GlobalDataStore
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# GlobalDataStore

An object that exposes methods to access a single data store.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

A **GlobalDataStore** exposes functions for saving and loading data for the
`Class.DataStoreService`.

See [Data stores](../../../cloud-services/data-stores/index.md) for an
in-depth guide on data structure, management, error handling, limits, and
more.

Ordered data stores do not support versioning and metadata, so
`Class.DataStoreKeyInfo` is always `nil` for keys in an
`Class.OrderedDataStore`. If you need versioning and metadata support, use a
`Class.DataStore`.

## Methods

### `Class.GlobalDataStore:GetAsync`

``GetAsync(key: `string`, options: `Class.DataStoreGetOptions`)`` -> `Tuple`
  [Yields]

### `Class.GlobalDataStore:IncrementAsync`

``IncrementAsync(key: `string`, delta: `int`, userIds: `Array`, options: `Class.DataStoreIncrementOptions`)`` -> `Variant`
  [Yields]

### `Class.GlobalDataStore:OnUpdate`

``OnUpdate(key: `string`, callback: `Datatype.Function`)`` -> `Datatype.RBXScriptConnection`
  [Deprecated]

### `Class.GlobalDataStore:RemoveAsync`

``RemoveAsync(key: `string`)`` -> `Tuple`
  [Yields]

### `Class.GlobalDataStore:SetAsync`

``SetAsync(key: `string`, value: `Variant`, userIds: `Array`, options: `Class.DataStoreSetOptions`)`` -> `Variant`
  [Yields]

### `Class.GlobalDataStore:UpdateAsync`

``UpdateAsync(key: `string`, transformFunction: `Datatype.Function`)`` -> `Tuple`
  [Yields]

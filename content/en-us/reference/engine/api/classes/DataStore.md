---
title: DataStore
type: class
superclass: GlobalDataStore
tags: [NotCreatable, NotReplicated]
---

# DataStore

**Inherits from:** `Class.GlobalDataStore` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

See [Data stores](../../../cloud-services/data-stores/index.md) for an
in-depth guide on data structure, management, error handling, limits, and
more.

## Methods

### `Class.DataStore:GetVersionAsync`

``GetVersionAsync(key: `string`, version: `string`)`` -> `Tuple`
  [Yields]

### `Class.DataStore:GetVersionAtTimeAsync`

``GetVersionAtTimeAsync(key: `string`, timestamp: `int64`)`` -> `Tuple`
  [Yields]

### `Class.DataStore:ListKeysAsync`

``ListKeysAsync(prefix: `string`, pageSize: `int`, cursor: `string`, excludeDeleted: `bool`)`` -> `Class.DataStoreKeyPages`
  [Yields]

### `Class.DataStore:ListVersionsAsync`

``ListVersionsAsync(key: `string`, sortDirection: `Enum.SortDirection`, minDate: `int64`, maxDate: `int64`, pageSize: `int`)`` -> `Class.DataStoreVersionPages`
  [Yields]

### `Class.DataStore:RemoveVersionAsync`

``RemoveVersionAsync(key: `string`, version: `string`)`` -> `null`
  [Yields] [Deprecated]

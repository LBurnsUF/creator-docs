---
title: DataStoreKeyInfo
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# DataStoreKeyInfo

An object specifying information about a particular version of the key.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

An object describing information about a particular version of the key. This
is returned as the second return value by `Class.GlobalDataStore:GetAsync()`,
`Class.GlobalDataStore:UpdateAsync()`,
`Class.GlobalDataStore:IncrementAsync()`,
`Class.GlobalDataStore:RemoveAsync()`, and
`Class.DataStore:GetVersionAsync()`.

See also:

- [Data Stores](../../../cloud-services/data-stores/index.md), an in-depth
  guide on data structure, management, error handling, etc.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.DataStoreKeyInfo.CreatedTime` | `int64` | [ReadOnly] [NotReplicated] |
| `Class.DataStoreKeyInfo.UpdatedTime` | `int64` | [ReadOnly] [NotReplicated] |
| `Class.DataStoreKeyInfo.Version` | `string` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.DataStoreKeyInfo:GetMetadata`

``GetMetadata()`` -> `Dictionary`

### `Class.DataStoreKeyInfo:GetUserIds`

``GetUserIds()`` -> `Array`

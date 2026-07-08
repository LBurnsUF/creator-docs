---
title: DataStoreInfo
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# DataStoreInfo

Object describing data store information.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

Object describing data store information such as name, created time, and time
last updated. This object is a member of the `Class.DataStoreListingPages`
object returned by `Class.DataStoreService:ListDataStoresAsync()`.

See also:

- [Data Stores](../../../cloud-services/data-stores/index.md), an in-depth
  guide on data structure, management, error handling, etc.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.DataStoreInfo.CreatedTime` | `int64` | [ReadOnly] [NotReplicated] |
| `Class.DataStoreInfo.DataStoreName` | `string` | [ReadOnly] [NotReplicated] |
| `Class.DataStoreInfo.UpdatedTime` | `int64` | [ReadOnly] [NotReplicated] |

---
title: DataStoreObjectVersionInfo
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# DataStoreObjectVersionInfo

An instance describing version information for a key.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

An instance describing version information for a key, including the version
string, created time, and whether it has been marked as deleted.

See also:

- [Data Stores](../../../cloud-services/data-stores/index.md), an in-depth
  guide on data structure, management, error handling, etc.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.DataStoreObjectVersionInfo.CreatedTime` | `int64` | [ReadOnly] [NotReplicated] |
| `Class.DataStoreObjectVersionInfo.IsDeleted` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.DataStoreObjectVersionInfo.Version` | `string` | [ReadOnly] [NotReplicated] |

---
title: DataStoreKey
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# DataStoreKey

Object representing a key on a `Class.DataStoreKeyPages` object.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

Object representing a key on a `Class.DataStoreKeyPages` object. It contains
the key name as `Class.DataStoreKey.KeyName`. This object is a member of the
`Class.DataStoreKeyPages` object returned by
`Class.DataStore:ListKeysAsync()`.

See also:

- [Data Stores](../../../cloud-services/data-stores/index.md), an in-depth
  guide on data structure, management, error handling, etc.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.DataStoreKey.KeyName` | `string` | [ReadOnly] [NotReplicated] |

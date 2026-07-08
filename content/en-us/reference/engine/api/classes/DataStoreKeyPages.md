---
title: DataStoreKeyPages
type: class
superclass: Pages
tags: [NotCreatable, NotReplicated]
---

# DataStoreKeyPages

A special type of `Class.Pages` object whose pages contain
`Class.DataStoreKey` instances.

**Inherits from:** `Class.Pages` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

A special type of `Class.Pages` object whose pages contain
`Class.DataStoreKey` instances. `Class.Pages:GetCurrentPage()` can be used to
retrieve an array of the `Class.DataStoreKey` instances.

See also:

- [Data Stores](../../../cloud-services/data-stores/index.md), an in-depth
  guide on data structure, management, error handling, etc.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.DataStoreKeyPages.Cursor` | `string` | [ReadOnly] [NotReplicated] |

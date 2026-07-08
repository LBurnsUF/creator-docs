---
title: DataStoreListingPages
type: class
superclass: Pages
tags: [NotCreatable, NotReplicated]
---

# DataStoreListingPages

A special type of `Class.Pages` object whose pages contain
`Class.DataStoreInfo` instances.

**Inherits from:** `Class.Pages` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

A special type of `Class.Pages` object whose pages contain
`Class.DataStoreInfo` instances. `Class.Pages:GetCurrentPage()` can be used to
retrieve an array of the `Class.DataStoreInfo` instances.

See also:

- [Data Stores](../../../cloud-services/data-stores/index.md), an in-depth
  guide on data structure, management, error handling, etc.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.DataStoreListingPages.Cursor` | `string` | [ReadOnly] [NotReplicated] |

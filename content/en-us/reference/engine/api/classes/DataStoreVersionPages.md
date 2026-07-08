---
title: DataStoreVersionPages
type: class
superclass: Pages
tags: [NotCreatable, NotReplicated]
---

# DataStoreVersionPages

A special type of `Class.Pages` object whose pages contain
`Class.DataStoreObjectVersionInfo` instances.

**Inherits from:** `Class.Pages` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Description

A special type of `Class.Pages` object whose pages contain
`Class.DataStoreObjectVersionInfo` instances from a `Class.GlobalDataStore`.
`Class.Pages:GetCurrentPage()` can be used to retrieve an array of the
`Class.DataStoreObjectVersionInfo` instances.

See also:

- [Data Stores](../../../cloud-services/data-stores/index.md), an in-depth
  guide on data structure, management, error handling, etc.

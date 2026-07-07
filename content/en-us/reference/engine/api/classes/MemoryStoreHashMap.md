---
title: MemoryStoreHashMap
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# MemoryStoreHashMap

**Inherits**: Instance > Object

**Tags**: NotCreatable, NotReplicated

## Methods

- **GetAsync**(`key: string`) -> `Variant` [Yields]
- **ListItemsAsync**(`count: int`) -> `MemoryStoreHashMapPages` [Yields]
- **RemoveAsync**(`key: string`) -> `null` [Yields]
- **SetAsync**(`key: string`, `value: Variant`, `expiration: int64`) -> `bool` [Yields]
- **UpdateAsync**(`key: string`, `transformFunction: Function`, `expiration: int64`) -> `Variant` [Yields]

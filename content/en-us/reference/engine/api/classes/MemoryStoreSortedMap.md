---
title: MemoryStoreSortedMap
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# MemoryStoreSortedMap

**Inherits**: Instance > Object

**Tags**: NotCreatable, NotReplicated

## Methods

- **GetAsync**(`key: string`) -> `Tuple` [Yields]
- **GetRangeAsync**(`direction: SortDirection`, `count: int`, `exclusiveLowerBound: Variant`, `exclusiveUpperBound: Variant`) -> `Array` [Yields]
- **GetSizeAsync**() -> `int` [Yields]
- **RemoveAsync**(`key: string`) -> `null` [Yields]
- **SetAsync**(`key: string`, `value: Variant`, `expiration: int64`, `sortKey: Variant`) -> `bool` [Yields]
- **UpdateAsync**(`key: string`, `transformFunction: Function`, `expiration: int64`) -> `Tuple` [Yields]

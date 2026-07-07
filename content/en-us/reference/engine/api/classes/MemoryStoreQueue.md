---
title: MemoryStoreQueue
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# MemoryStoreQueue

**Inherits**: Instance > Object

**Tags**: NotCreatable, NotReplicated

## Methods

- **AddAsync**(`value: Variant`, `expiration: int64`, `priority: double = 0`) -> `null` [Yields]
- **GetSizeAsync**(`excludeInvisible: bool = false`) -> `int` [Yields]
- **ReadAsync**(`count: int`, `allOrNothing: bool = false`, `waitTimeout: double = -1`) -> `Tuple` [Yields]
- **RemoveAsync**(`id: string`) -> `null` [Yields]

---
title: GlobalDataStore
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# GlobalDataStore

**Inherits**: Instance > Object

**Tags**: NotCreatable, NotReplicated

## Methods

- **GetAsync**(`key: string`, `options: DataStoreGetOptions = nil`) -> `Tuple` [Yields]
- **IncrementAsync**(`key: string`, `delta: int = 1`, `userIds: Array = {}`, `options: DataStoreIncrementOptions = nil`) -> `Variant` [Yields]
- **OnUpdate**(`key: string`, `callback: Function`) -> `RBXScriptConnection` [Deprecated]
- **RemoveAsync**(`key: string`) -> `Tuple` [Yields]
- **SetAsync**(`key: string`, `value: Variant`, `userIds: Array = {}`, `options: DataStoreSetOptions = nil`) -> `Variant` [Yields]
- **UpdateAsync**(`key: string`, `transformFunction: Function`) -> `Tuple` [Yields]

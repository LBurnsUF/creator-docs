---
title: DataStore
type: class
superclass: GlobalDataStore
tags: [NotCreatable, NotReplicated]
---

# DataStore

**Inherits**: GlobalDataStore > Instance > Object

**Tags**: NotCreatable, NotReplicated

## Methods

- **GetVersionAsync**(`key: string`, `version: string`) -> `Tuple` [Yields]
- **GetVersionAtTimeAsync**(`key: string`, `timestamp: int64`) -> `Tuple` [Yields]
- **ListKeysAsync**(`prefix: string = `, `pageSize: int = 0`, `cursor: string = `, `excludeDeleted: bool = false`) -> `DataStoreKeyPages` [Yields]
- **ListVersionsAsync**(`key: string`, `sortDirection: SortDirection = Ascending`, `minDate: int64 = 0`, `maxDate: int64 = 0`, `pageSize: int = 0`) -> `DataStoreVersionPages` [Yields]
- **RemoveVersionAsync**(`key: string`, `version: string`) -> `null` [Yields] [Deprecated]

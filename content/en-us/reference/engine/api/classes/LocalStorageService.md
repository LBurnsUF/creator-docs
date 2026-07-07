---
title: LocalStorageService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# LocalStorageService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **Flush**() -> `null`
- **GetItem**(`key: string`) -> `string`
- **SetItem**(`key: string`, `value: string`) -> `null`
- **WhenLoaded**(`callback: Function`) -> `null`

## Events

- **ItemWasSet**(`key: string`, `value: string`)
- **StoreWasCleared**()

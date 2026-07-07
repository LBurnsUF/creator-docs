---
title: MemStorageService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# MemStorageService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **Bind**(`key: string`, `callback: Function`) -> `MemStorageConnection`
- **BindAndFire**(`key: string`, `callback: Function`) -> `MemStorageConnection`
- **Call**(`key: string`, `input: Variant`) -> `Variant`
- **Fire**(`key: string`, `value: string = `) -> `null`
- **GetItem**(`key: string`, `defaultValue: string = `) -> `string`
- **HasItem**(`key: string`) -> `bool`
- **RemoveItem**(`key: string`) -> `bool`
- **SetItem**(`key: string`, `value: string = `) -> `null`

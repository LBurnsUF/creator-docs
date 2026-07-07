---
title: ConfigService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ConfigService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **ClearTestingValue**(`key: string`) -> `null`
- **GetConfigAsync**() -> `ConfigSnapshot` [Yields]
- **GetConfigForPlayerAsync**(`player: Player`) -> `ConfigSnapshot` [Yields]
- **SetTestingValue**(`key: string`, `value: Variant`) -> `null`

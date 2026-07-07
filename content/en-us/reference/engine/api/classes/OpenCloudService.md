---
title: OpenCloudService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated, Deprecated]
---

# OpenCloudService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated, Deprecated

## Methods

- **GetApiV1**() -> `OpenCloudApiV1` [Deprecated]
- **HttpRequestAsync**(`options: Dictionary`) -> `Dictionary` [Yields]
- **InvokeAsync**(`version: string`, `methodName: string`, `arguments: Dictionary`, `headers: Dictionary = nil`) -> `Dictionary` [Yields] [Deprecated]
- **RegisterOpenCloud**(`version: string`, `methodName: string`, `method: Function`) -> `null`
- **RegistrationComplete**() -> `null`

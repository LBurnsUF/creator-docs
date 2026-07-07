---
title: LinkingService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# LinkingService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **DetectUrl**(`url: string`) -> `null`
- **GetAndClearLastPendingUrl**() -> `Dictionary`
- **GetLastLuaUrl**() -> `string?`
- **IsUrlRegistered**(`url: string`) -> `bool`
- **OpenUrl**(`url: string`) -> `bool` [Yields]
- **RegisterLuaUrl**(`url: string`) -> `null`
- **StartLuaUrlDelivery**() -> `Dictionary?`
- **StopLuaUrlDelivery**() -> `null`
- **SupportsSwitchToSettingsApp**() -> `bool` [Yields]
- **SwitchToSettingsApp**(`route: string?`) -> `null` [Yields]

## Events

- **OnLuaUrl**(`url: string`, `matchedUrl: string`, `attributionUrl: string?`)

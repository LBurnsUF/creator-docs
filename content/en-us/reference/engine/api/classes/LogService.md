---
title: LogService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# LogService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **ClearOutput**() -> `null`
- **Error**(`message: string`, `context: Dictionary = nil`) -> `null` [CustomLuaState]
- **ExecuteScript**(`source: string`) -> `null`
- **GetHttpResultHistory**() -> `Array`
- **GetLogHistory**() -> `Array`
- **Info**(`message: string`, `context: Dictionary = nil`) -> `null` [CustomLuaState]
- **Log**(`messageType: MessageType`, `message: string`, `context: Dictionary = nil`) -> `null` [CustomLuaState]
- **Output**(`message: string`, `context: Dictionary = nil`) -> `null` [CustomLuaState]
- **RequestHttpResultApproved**() -> `null`
- **RequestServerHttpResult**() -> `null`
- **RequestServerOutput**() -> `null`
- **Warn**(`message: string`, `context: Dictionary = nil`) -> `null` [CustomLuaState]

## Events

- **HttpResultOut**(`httpResult: Dictionary`)
- **MessageOut**(`message: string`, `messageType: MessageType`, `context: Dictionary`)
- **OnHttpResultApproved**(`isApproved: bool`)
- **ServerContextOut**(`contextData: Dictionary`)
- **ServerHttpResultOut**(`httpResult: Dictionary`)
- **ServerMessageOut**(`message: string`, `messageType: MessageType`, `timestamp: double`)

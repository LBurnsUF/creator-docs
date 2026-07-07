---
title: LogService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# LogService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.LogService:ClearOutput`

``ClearOutput()`` → `null`

### `Class.LogService:Error`

``Error(message: `string`, context: `Dictionary`)`` → `null`
  [CustomLuaState]

### `Class.LogService:ExecuteScript`

``ExecuteScript(source: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.LogService:GetHttpResultHistory`

``GetHttpResultHistory()`` → `Array`
   {security: RobloxScriptSecurity}

### `Class.LogService:GetLogHistory`

``GetLogHistory()`` → `Array`

### `Class.LogService:Info`

``Info(message: `string`, context: `Dictionary`)`` → `null`
  [CustomLuaState]

### `Class.LogService:Log`

``Log(messageType: `Enum.MessageType`, message: `string`, context: `Dictionary`)`` → `null`
  [CustomLuaState]

### `Class.LogService:Output`

``Output(message: `string`, context: `Dictionary`)`` → `null`
  [CustomLuaState]

### `Class.LogService:RequestHttpResultApproved`

``RequestHttpResultApproved()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.LogService:RequestServerHttpResult`

``RequestServerHttpResult()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.LogService:RequestServerOutput`

``RequestServerOutput()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.LogService:Warn`

``Warn(message: `string`, context: `Dictionary`)`` → `null`
  [CustomLuaState]

## Events

### `Class.LogService.HttpResultOut`

Fires with: (httpResult: `Dictionary`)

### `Class.LogService.MessageOut`

Fires with: (message: `string`, messageType: `Enum.MessageType`, context: `Dictionary`)

### `Class.LogService.OnHttpResultApproved`

Fires with: (isApproved: `bool`)

### `Class.LogService.ServerContextOut`

Fires with: (contextData: `Dictionary`)

### `Class.LogService.ServerHttpResultOut`

Fires with: (httpResult: `Dictionary`)

### `Class.LogService.ServerMessageOut`

Fires with: (message: `string`, messageType: `Enum.MessageType`, timestamp: `double`)

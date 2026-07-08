---
title: LogService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# LogService

A service that allows you to read outputted text.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

`LogService` allows you to log structured log entries and read outputted text.

#### Template Syntax

Methods that accept a `context` table support `{key}` template placeholders in
the message string. To include a literal brace character in the output, use
double braces: `{{` produces a literal `{` and `}}` produces a literal `}`.

```lua
local LogService = game:GetService("LogService")

LogService:Info("Value = {{result}}: {val}", {val = 42})
-- Output: "Value = {result}: 42"
```

#### Warning

This service might have unexpected or unreliable behavior and content might be
truncated. Don't rely on contents of events and messages emitted by this
service for any important game logic.

## Methods

### `Class.LogService:ClearOutput`

``ClearOutput()`` -> `null`

### `Class.LogService:Error`

``Error(message: `string`, context: `Dictionary`)`` -> `null`
  [CustomLuaState]

### `Class.LogService:ExecuteScript`

``ExecuteScript(source: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.LogService:GetHttpResultHistory`

``GetHttpResultHistory()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.LogService:GetLogHistory`

``GetLogHistory()`` -> `Array`

### `Class.LogService:Info`

``Info(message: `string`, context: `Dictionary`)`` -> `null`
  [CustomLuaState]

### `Class.LogService:Log`

``Log(messageType: `Enum.MessageType`, message: `string`, context: `Dictionary`)`` -> `null`
  [CustomLuaState]

### `Class.LogService:Output`

``Output(message: `string`, context: `Dictionary`)`` -> `null`
  [CustomLuaState]

### `Class.LogService:RequestHttpResultApproved`

``RequestHttpResultApproved()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.LogService:RequestServerHttpResult`

``RequestServerHttpResult()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.LogService:RequestServerOutput`

``RequestServerOutput()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.LogService:Warn`

``Warn(message: `string`, context: `Dictionary`)`` -> `null`
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

---
title: ScriptDebuggerService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ScriptDebuggerService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.ScriptDebuggerService:AddBreakpoint`

``AddBreakpoint(scriptInstance: `Class.LuaSourceContainer`, breakpoint: `Dictionary`)`` → `Dictionary`
   {security: PluginSecurity}

### `Class.ScriptDebuggerService:ClearBreakpoints`

``ClearBreakpoints()`` → `null`
   {security: PluginSecurity}

### `Class.ScriptDebuggerService:Evaluate`

``Evaluate(expression: `string`, frameId: `int?`)`` → `Dictionary`
   {security: PluginSecurity}

### `Class.ScriptDebuggerService:GetRootVariables`

``GetRootVariables(frameId: `int`)`` → `Array`
   {security: PluginSecurity}

### `Class.ScriptDebuggerService:GetStackTrace`

``GetStackTrace(threadId: `int`, startFrame: `int?`)`` → `Dictionary`
   {security: PluginSecurity}

### `Class.ScriptDebuggerService:GetThreads`

``GetThreads()`` → `Array`
   {security: PluginSecurity}

### `Class.ScriptDebuggerService:GetVariables`

``GetVariables(variablesReference: `int`)`` → `Array`
   {security: PluginSecurity}

### `Class.ScriptDebuggerService:Pause`

``Pause()`` → `null`
   {security: PluginSecurity}

### `Class.ScriptDebuggerService:RemoveBreakpoint`

``RemoveBreakpoint(scriptInstance: `Class.LuaSourceContainer`, line: `int`)`` → `bool`
   {security: PluginSecurity}

### `Class.ScriptDebuggerService:SetExceptionBreakMode`

``SetExceptionBreakMode(breakMode: `Enum.DebugBreakModeType`)`` → `null`
   {security: PluginSecurity}

## Events

### `Class.ScriptDebuggerService.Resumed`

Fires with: (threadIds: `Array`)

## Callbacks

### `Class.ScriptDebuggerService.OnStopped`

``OnStopped(stopped: `Dictionary`)`` → `Dictionary`

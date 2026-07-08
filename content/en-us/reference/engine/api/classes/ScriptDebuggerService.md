---
title: ScriptDebuggerService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ScriptDebuggerService

Provides programmatic breakpoint management, execution control, and runtime
inspection of Luau scripts during a playtest.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

`ScriptDebuggerService` exposes the Roblox Studio Luau debugger for
programmatic use. It provides functionality for breakpoint management,
execution control, and runtime state inspection.

**APIs in this class are currently in beta and are subject to breaking
changes.**

#### Breakpoint Propagation

Breakpoints set in the **edit** `Class.DataModel` are set on the specific
script instance and do not propagate to clones, but they propagate to
corresponding scripts in play data models at the start of a playtest.
Breakpoints set in a **play** `Class.DataModel` propagate to script clones in
the same data model and to corresponding scripts in other data models.

#### Parallel Threads

The behavior of this API with parallel Luau is undefined.

## Methods

### `Class.ScriptDebuggerService:AddBreakpoint`

``AddBreakpoint(scriptInstance: `Class.LuaSourceContainer`, breakpoint: `Dictionary`)`` -> `Dictionary`
   {security: PluginSecurity}

### `Class.ScriptDebuggerService:ClearBreakpoints`

``ClearBreakpoints()`` -> `null`
   {security: PluginSecurity}

### `Class.ScriptDebuggerService:Evaluate`

``Evaluate(expression: `string`, frameId: `int?`)`` -> `Dictionary`
   {security: PluginSecurity}

### `Class.ScriptDebuggerService:GetRootVariables`

``GetRootVariables(frameId: `int`)`` -> `Array`
   {security: PluginSecurity}

### `Class.ScriptDebuggerService:GetStackTrace`

``GetStackTrace(threadId: `int`, startFrame: `int?`)`` -> `Dictionary`
   {security: PluginSecurity}

### `Class.ScriptDebuggerService:GetThreads`

``GetThreads()`` -> `Array`
   {security: PluginSecurity}

### `Class.ScriptDebuggerService:GetVariables`

``GetVariables(variablesReference: `int`)`` -> `Array`
   {security: PluginSecurity}

### `Class.ScriptDebuggerService:Pause`

``Pause()`` -> `null`
   {security: PluginSecurity}

### `Class.ScriptDebuggerService:RemoveBreakpoint`

``RemoveBreakpoint(scriptInstance: `Class.LuaSourceContainer`, line: `int`)`` -> `bool`
   {security: PluginSecurity}

### `Class.ScriptDebuggerService:SetExceptionBreakMode`

``SetExceptionBreakMode(breakMode: `Enum.DebugBreakModeType`)`` -> `null`
   {security: PluginSecurity}

## Events

### `Class.ScriptDebuggerService.Resumed`

Fires with: (threadIds: `Array`)

## Callbacks

### `Class.ScriptDebuggerService.OnStopped`

``OnStopped(stopped: `Dictionary`)`` -> `Dictionary`

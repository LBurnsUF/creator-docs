---
title: DebuggerConnection
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# DebuggerConnection

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.DebuggerConnection.ErrorMessage` | `string` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.DebuggerConnection.HasError` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.DebuggerConnection.Id` | `int` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.DebuggerConnection.IsPaused` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |

## Methods

### `Class.DebuggerConnection:AddBreakpoint`

``AddBreakpoint(script: `string`, line: `int`, breakpoint: `Class.Breakpoint`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.DebuggerConnection:Close`

``Close()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.DebuggerConnection:EvaluateWatch`

``EvaluateWatch(expression: `string`, frame: `Class.StackFrame`, callback: `Datatype.Function`)`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.DebuggerConnection:GetFrameById`

``GetFrameById(id: `int`)`` -> `Class.StackFrame`
   {security: RobloxScriptSecurity}

### `Class.DebuggerConnection:GetSource`

``GetSource(scriptRef: `string`, status: `Datatype.Function`)`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.DebuggerConnection:GetThreadById`

``GetThreadById(id: `int`)`` -> `Class.ThreadState`
   {security: RobloxScriptSecurity}

### `Class.DebuggerConnection:GetThreads`

``GetThreads(callback: `Datatype.Function`)`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.DebuggerConnection:GetVariableById`

``GetVariableById(id: `int`)`` -> `Class.DebuggerVariable`
   {security: RobloxScriptSecurity}

### `Class.DebuggerConnection:Pause`

``Pause(thread: `Class.ThreadState`, status: `Datatype.Function`)`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.DebuggerConnection:Populate`

``Populate(instance: `Class.Instance`, callback: `Datatype.Function`)`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.DebuggerConnection:RemoveBreakpoint`

``RemoveBreakpoint(breakpoint: `Class.Breakpoint`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.DebuggerConnection:Resume`

``Resume(thread: `Class.ThreadState`, status: `Datatype.Function`)`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.DebuggerConnection:SetExceptionBreakMode`

``SetExceptionBreakMode(breakMode: `Enum.DebuggerExceptionBreakMode`, callback: `Datatype.Function`)`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.DebuggerConnection:SetVariable`

``SetVariable(variable: `Class.DebuggerVariable`, value: `string`, callback: `Datatype.Function`)`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.DebuggerConnection:Step`

``Step(thread: `Class.ThreadState`, callback: `Datatype.Function`)`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.DebuggerConnection:StepIn`

``StepIn(thread: `Class.ThreadState`, callback: `Datatype.Function`)`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.DebuggerConnection:StepOut`

``StepOut(thread: `Class.ThreadState`, callback: `Datatype.Function`)`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.DebuggerConnection:UpdateSelectedFrame`

``UpdateSelectedFrame(threadId: `int`, frameNumber: `int`)`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.DebuggerConnection.BreakpointAdded`

Fires with: (breakpoint: `Class.Breakpoint`)

### `Class.DebuggerConnection.BreakpointChanged`

Fires with: (breakpoint: `Class.Breakpoint`)

### `Class.DebuggerConnection.BreakpointRemoved`

Fires with: (breakpoint: `Class.Breakpoint`, reason: `Enum.BreakpointRemoveReason`)

### `Class.DebuggerConnection.Paused`

Fires with: (pausedState: `Class.PausedState`, reason: `Enum.DebuggerPauseReason`)

### `Class.DebuggerConnection.Resumed`

Fires with: (pausedState: `Class.PausedState`)

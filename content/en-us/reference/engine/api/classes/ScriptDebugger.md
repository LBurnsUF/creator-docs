---
title: ScriptDebugger
type: class
superclass: Instance
tags: [NotCreatable]
---

# ScriptDebugger

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.ScriptDebugger.CurrentLine` | `int` | [ReadOnly] [NotReplicated] |
| `Class.ScriptDebugger.IsDebugging` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.ScriptDebugger.IsPaused` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.ScriptDebugger.Script` | `Class.Instance` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.ScriptDebugger:AddWatch`

``AddWatch(expression: `string`)`` → `Class.Instance`

### `Class.ScriptDebugger:GetBreakpoints`

``GetBreakpoints()`` → `Datatype.Instances`

### `Class.ScriptDebugger:GetGlobals`

``GetGlobals(stackFrame: `int`)`` → `Map`

### `Class.ScriptDebugger:GetLocals`

``GetLocals(stackFrame: `int`)`` → `Map`

### `Class.ScriptDebugger:GetStack`

``GetStack()`` → `Array`

### `Class.ScriptDebugger:GetUpvalues`

``GetUpvalues(stackFrame: `int`)`` → `Map`

### `Class.ScriptDebugger:GetWatchValue`

``GetWatchValue(watch: `Class.Instance`)`` → `Variant`

### `Class.ScriptDebugger:GetWatches`

``GetWatches()`` → `Datatype.Instances`

### `Class.ScriptDebugger:SetBreakpoint`

``SetBreakpoint(line: `int`, isContextDependentBreakpoint: `bool`)`` → `Class.Instance`

### `Class.ScriptDebugger:SetGlobal`

``SetGlobal(name: `string`, value: `Variant`, stackFrame: `int`)`` → `null`

### `Class.ScriptDebugger:SetLocal`

``SetLocal(name: `string`, value: `Variant`, stackFrame: `int`)`` → `null`

### `Class.ScriptDebugger:SetUpvalue`

``SetUpvalue(name: `string`, value: `Variant`, stackFrame: `int`)`` → `null`

## Events

### `Class.ScriptDebugger.BreakpointAdded`

Fires with: (breakpoint: `Class.Instance`)

### `Class.ScriptDebugger.BreakpointRemoved`

Fires with: (breakpoint: `Class.Instance`)

### `Class.ScriptDebugger.EncounteredBreak`

Fires with: (line: `int`, breakReason: `Enum.BreakReason`)

### `Class.ScriptDebugger.Resuming`

Fires with: ()

### `Class.ScriptDebugger.WatchAdded`

Fires with: (watch: `Class.Instance`)

### `Class.ScriptDebugger.WatchRemoved`

Fires with: (watch: `Class.Instance`)

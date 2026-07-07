---
title: MetaBreakpointManager
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# MetaBreakpointManager

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.MetaBreakpointManager:AddBreakpoint`

``AddBreakpoint(script: `Class.Instance`, line: `int`, condition: `Class.Instance`)`` → `Class.Instance`
   {security: RobloxScriptSecurity}

### `Class.MetaBreakpointManager:GetBreakpointById`

``GetBreakpointById(metaBreakpointId: `int`)`` → `Class.MetaBreakpoint`
   {security: RobloxScriptSecurity}

### `Class.MetaBreakpointManager:RemoveBreakpointById`

``RemoveBreakpointById(metaBreakpointId: `int`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.MetaBreakpointManager.MetaBreakpointAdded`

Fires with: (breakpoint: `Class.MetaBreakpoint`)

### `Class.MetaBreakpointManager.MetaBreakpointChanged`

Fires with: (breakpoint: `Class.MetaBreakpoint`)

### `Class.MetaBreakpointManager.MetaBreakpointRemoved`

Fires with: (breakpoint: `Class.MetaBreakpoint`)

### `Class.MetaBreakpointManager.MetaBreakpointSetChanged`

Fires with: (breakpoint: `Class.MetaBreakpoint`, detail: `Dictionary`)

---
title: MetaBreakpointManager
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# MetaBreakpointManager

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **AddBreakpoint**(`script: Instance`, `line: int`, `condition: Instance`) -> `Instance`
- **GetBreakpointById**(`metaBreakpointId: int`) -> `MetaBreakpoint`
- **RemoveBreakpointById**(`metaBreakpointId: int`) -> `null`

## Events

- **MetaBreakpointAdded**(`breakpoint: MetaBreakpoint`)
- **MetaBreakpointChanged**(`breakpoint: MetaBreakpoint`)
- **MetaBreakpointRemoved**(`breakpoint: MetaBreakpoint`)
- **MetaBreakpointSetChanged**(`breakpoint: MetaBreakpoint`, `detail: Dictionary`)

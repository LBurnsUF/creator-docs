---
title: DebuggerConnectionManager
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# DebuggerConnectionManager

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **Timeout**: `double` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **ConnectLocal**(`dataModel: DataModel`) -> `int`
- **FocusConnection**(`connection: DebuggerConnection`) -> `null`
- **GetAvailableConnection**() -> `DebuggerConnection`
- **GetConnectionById**(`id: int`) -> `DebuggerConnection`

## Events

- **ConnectionEnded**(`connection: DebuggerConnection`, `reason: DebuggerEndReason`)
- **ConnectionStarted**(`connection: DebuggerConnection`)
- **FocusChanged**(`connection: DebuggerConnection`)

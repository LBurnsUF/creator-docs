---
title: MetaBreakpoint
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# MetaBreakpoint

**Inherits**: Instance > Object

**Tags**: NotCreatable, NotReplicated

## Properties

- **Condition**: `string` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **ContinueExecution**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Enabled**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Id**: `int` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **IsLogpoint**: `bool` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Line**: `int` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **LogMessage**: `string` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **RemoveOnHit**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Script**: `string` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Valid**: `bool` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **GetContextBreakpoints**() -> `Dictionary`
- **Remove**(`status: Function`) -> `int`
- **SetChildBreakpointEnabledByScriptAndContext**(`script: string`, `contextGST: int`, `enabled: bool`) -> `null`
- **SetContextEnabled**(`context: int`, `enabled: bool`) -> `null`
- **SetContinueExecution**(`enabled: bool`) -> `null`
- **SetEnabled**(`enabled: bool`) -> `null`
- **SetLine**(`line: int`, `status: Function`) -> `int`
- **SetRemoveOnHit**(`enabled: bool`) -> `null`

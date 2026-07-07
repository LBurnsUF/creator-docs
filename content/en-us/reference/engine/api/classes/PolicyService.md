---
title: PolicyService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# PolicyService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **IsLuobuServer**: `TriStateBoolean` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **LuobuWhitelisted**: `TriStateBoolean` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **CanViewBrandProjectAsync**(`player: Player`, `brandProjectId: string`) -> `bool` [Yields]
- **GetPolicyInfoForPlayerAsync**(`player: Instance`) -> `Dictionary` [Yields]
- **GetPolicyInfoForServerRobloxOnlyAsync**() -> `Dictionary` [Yields]

---
title: StudioTestService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# StudioTestService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **EditModeActive**: `bool` (Security: Read=PluginSecurity, Write=PluginSecurity)

## Methods

- **AddPlayers**(`numPlayers: int`) -> `null`
- **CanLeaveTest**() -> `bool`
- **EndTest**(`value: Variant`) -> `null`
- **ExecuteMultiplayerTestAsync**(`numPlayers: int`, `args: Variant`) -> `Variant` [Yields]
- **ExecutePlayModeAsync**(`args: Variant`) -> `Variant` [Yields]
- **ExecuteRunModeAsync**(`args: Variant`) -> `Variant` [Yields]
- **GetTestArgs**() -> `Variant`
- **LeaveTest**() -> `null`

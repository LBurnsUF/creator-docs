---
title: RemoteCommandService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# RemoteCommandService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Methods

- **ExecuteCommand**(`code: string`, `args: Tuple`) -> `ExecutedRemoteCommand`
- **ExecuteCommandAsync**(`code: string`, `args: Tuple`) -> `Tuple` [Yields]
- **GetExecutingPlayer**() -> `Player`
- **GetReceivedUpdateSignal**() -> `RBXScriptSignal`
- **GetStoppingSignal**() -> `RBXScriptSignal`
- **SendUpdate**(`args: Tuple`) -> `null`

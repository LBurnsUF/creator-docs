---
title: RemoteFunction
type: class
superclass: Instance
---

# RemoteFunction

**Inherits**: Instance > Object

## Methods

- **InvokeClient**(`player: Player`, `arguments: Tuple`) -> `Tuple` [Yields]
- **InvokeServer**(`arguments: Tuple`) -> `Tuple` [Yields]

## Callbacks

- **OnClientInvoke**(`arguments: Tuple`) -> `Tuple`
- **OnServerInvoke**(`player: Player`, `arguments: Tuple`) -> `Tuple`

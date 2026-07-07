---
title: RemoteCommandService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# RemoteCommandService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Methods

### `Class.RemoteCommandService:ExecuteCommand`

``ExecuteCommand(code: `string`, args: `Tuple`)`` → `Class.ExecutedRemoteCommand`
   {security: RobloxScriptSecurity}

### `Class.RemoteCommandService:ExecuteCommandAsync`

``ExecuteCommandAsync(code: `string`, args: `Tuple`)`` → `Tuple`
  [Yields] {security: RobloxScriptSecurity}

### `Class.RemoteCommandService:GetExecutingPlayer`

``GetExecutingPlayer()`` → `Class.Player`

### `Class.RemoteCommandService:GetReceivedUpdateSignal`

``GetReceivedUpdateSignal()`` → `Datatype.RBXScriptSignal`

### `Class.RemoteCommandService:GetStoppingSignal`

``GetStoppingSignal()`` → `Datatype.RBXScriptSignal`

### `Class.RemoteCommandService:SendUpdate`

``SendUpdate(args: `Tuple`)`` → `null`

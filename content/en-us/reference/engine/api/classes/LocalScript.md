---
title: LocalScript
type: class
superclass: Script
---

# LocalScript

An object that contains and runs Luau code on the client (player's device)
instead of the server.

**Inherits from:** `Class.Script` > `Class.BaseScript` > `Class.LuaSourceContainer` > `Class.Instance` > `Class.Object`

## Description

A `Class.LocalScript` is a Luau source container that runs its contents on the
client (player's device) instead of the server. It is used to access
client-only objects such as the player's `Class.Camera`.

For code run through `Class.LocalScript|LocalScripts`, the
`Class.Players.LocalPlayer|LocalPlayer` property of the `Class.Players`
service will return the player whose client is running the script.

See [here](../../../projects/data-model.md#client) for a table of valid
container services from which `Class.LocalScript|LocalScripts` will execute.

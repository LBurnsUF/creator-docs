---
title: ReplicatedStorage
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# ReplicatedStorage

A container service for objects that are replicated to all clients.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Description

`Class.ReplicatedStorage` is a general container service for objects that are
available to both the server and connected clients. It is ideal for
`Class.ModuleScript`, `Class.RemoteFunction`, `Class.RemoteEvent`, and other
objects that are useful to both server-side `Class.Script|Scripts` and
client-side `Class.LocalScript|LocalScripts`.

Objects parented to this service are fully replicated to clients, and normal
replication rules apply. Any changes that are made on the client persist but
aren't replicated to the server. Client changes may be overwritten if the
server does something that overwrites those changes.

Certain changes on the client, such as moving an object from the
`Class.Workspace` to `Class.ReplicatedStorage`, can lead to desynchronization
issues (for example, physics updates not being replicated to the object).

`Class.LocalScript|LocalScripts` do not run when parented to this service,
even if they are `Class.BaseScript.Enabled|Enabled`;
`Class.LocalScript|LocalScripts` have various other locations where they
eventually run on a `Class.Player` client such as
`Class.StarterPlayerScripts`, `Class.StarterCharacterScripts`, or
`Class.StarterGui`.

Similarly, `Class.Script|Scripts` do not run when parented to this service
unless you change their `Enum.RunContext` property from the default value of
`Enum.RunContext.Legacy|Legacy`. Server `Class.Script|Scripts` that run on
their own should be parented to `Class.ServerScriptService` instead.

If a `Class.ModuleScript` within this service is required by any other script,
it runs as normal. Such modules typically house code that is shared by the
server and client.

---
title: RemoteEvent
type: class
superclass: BaseRemoteEvent
---

# RemoteEvent

An object which facilitates asynchronous, one-way communication across the
client-server boundary. Scripts firing a `Class.RemoteEvent` do not yield.

**Inherits from:** `Class.BaseRemoteEvent` > `Class.Instance` > `Class.Object`

## Description

The **RemoteEvent** object facilitates asynchronous, one-way communication
across the [client-server](../../../projects/client-server.md) boundary
without yielding for a response. This communication can be directed from one
client to the server, from the server to a specific client, or from the server
to all clients.

In order for both the server and clients to access a `Class.RemoteEvent`
instance, it must be in a place where both sides can see it, such as
`Class.ReplicatedStorage`, although in some cases it's appropriate to store it
in `Class.Workspace` or inside a `Class.Tool`.

If no connected listener exists to handle an event, you might see a
`Remote event invocation discarded` error in the log to indicate that the
event was discarded and that you need to implement either `OnClientEvent` or
`OnServerEvent`. Unlike `Class.UnreliableRemoteEvent|UnreliableRemoteEvents`,
`Class.RemoteEvent|RemoteEvents` buffer a large number of events before
throwing this error.

If you need the result of the call, you should use a `Class.RemoteFunction`
instead. Otherwise a remote event is recommended since it will minimize
network traffic/latency and won't yield the script to wait for a response.

See [Remote events and callbacks](../../../scripting/events/remote.md) for
code samples and further details.

#### Throttling

Remote events are subject to rate limits when sent from the client to the
server with the `Class.RemoteEvent:FireServer()|FireServer()` method.
`Class.RemoteEvent|RemoteEvents` and
`Class.UnreliableRemoteEvent|UnreliableRemoteEvents` both have a limit of
approximately 500 requests per second, per client. This limit is **shared
among all remote events of the same type**. To avoid throttling and latency
issues, limit recurring remote events whenever possible.

#### Parameter limitations

Any type of Roblox object (`Datatype.Enum`, `Class.Instance`, etc.) can be
passed as a parameter when a `Class.RemoteEvent` is fired, as well as Luau
types such as numbers, strings, and booleans, although you should carefully
explore the
[limitations](../../../scripting/events/remote.md#argument-limitations).

## Methods

### `Class.RemoteEvent:FireAllClients`

``FireAllClients(arguments: `Tuple`)`` -> `null`

### `Class.RemoteEvent:FireClient`

``FireClient(player: `Class.Player`, arguments: `Tuple`)`` -> `null`

### `Class.RemoteEvent:FireServer`

``FireServer(arguments: `Tuple`)`` -> `null`

## Events

### `Class.RemoteEvent.OnClientEvent`

Fires with: (arguments: `Tuple`)

### `Class.RemoteEvent.OnServerEvent`

Fires with: (player: `Class.Player`, arguments: `Tuple`)

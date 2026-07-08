---
title: UnreliableRemoteEvent
type: class
superclass: BaseRemoteEvent
---

# UnreliableRemoteEvent

An object which facilitates asynchronous, unordered and unreliable, one-way
communication across the client-server boundary. Scripts firing a
`Class.UnreliableRemoteEvent` do not yield.

**Inherits from:** `Class.BaseRemoteEvent` > `Class.Instance` > `Class.Object`

## Description

The **UnreliableRemoteEvent** object is a variant of the `Class.RemoteEvent`
object. It facilitates asynchronous, unordered and unreliable, one-way
communication across the [client-server](../../../projects/client-server.md)
boundary without yielding for a response. This communication can be directed
from one client to the server, from the server to a specific client, or from
the server to all clients.

In order for both the server and clients to access a
`Class.UnreliableRemoteEvent` instance, it must be in a place where both sides
can see it, such as `Class.ReplicatedStorage`, although in some cases it's
appropriate to store it in `Class.Workspace` or inside a `Class.Tool`.

`Class.UnreliableRemoteEvent` is best used for ephemeral events, including
effects that are only relevant for a short time, or for replicating
continuously changing data. These events are not resent if they are lost and
they do not wait for previously fired events to arrive before being processed,
potentially resulting in reduced latency and network traffic. When you need
ordering and reliability, use a `Class.RemoteEvent` instead.

If no connected listener exists to handle an event, you might see a
`Remote event invocation discarded` error in the log to indicate that the
event was discarded and that you need to implement either `OnClientEvent` or
`OnServerEvent`.

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
passed as a parameter when an `Class.UnreliableRemoteEvent` is fired, as well
as Luau types such as numbers, strings, and booleans, although you should
carefully explore the
[limitations](../../../scripting/events/remote.md#argument-limitations).

Events with payloads larger than 1000 bytes are dropped. When this happens in
Studio, a log message in the [Output](../../../studio/output.md) window
indicates the number of bytes the event went over.

Like all events, the `Class.UnreliableRemoteEvent` methods encode and compress
certain object types, such as buffers, which shrinks the payload size and can
make it difficult to verify whether you are under the limit prior to firing
the event. If you frequently reach this limit, consider whether a standard
`Class.RemoteEvent` is the better fit for your use case.

## Methods

### `Class.UnreliableRemoteEvent:FireAllClients`

``FireAllClients(arguments: `Tuple`)`` -> `null`

### `Class.UnreliableRemoteEvent:FireClient`

``FireClient(player: `Class.Player`, arguments: `Tuple`)`` -> `null`

### `Class.UnreliableRemoteEvent:FireServer`

``FireServer(arguments: `Tuple`)`` -> `null`

## Events

### `Class.UnreliableRemoteEvent.OnClientEvent`

Fires with: (arguments: `Tuple`)

### `Class.UnreliableRemoteEvent.OnServerEvent`

Fires with: (player: `Class.Player`, arguments: `Tuple`)

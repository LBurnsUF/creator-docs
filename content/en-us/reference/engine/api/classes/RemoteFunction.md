---
title: RemoteFunction
type: class
superclass: Instance
---

# RemoteFunction

An object which facilitates synchronous, two-way communication across the
client-server boundary. Scripts invoking a `Class.RemoteFunction` yield until
they receive a response from the recipient.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

The **RemoteFunction** object facilitates synchronous, two-way communication
across the [client-server](../../../projects/client-server.md) boundary. You
can use it to define a custom callback function and invoke it manually by
calling `Class.RemoteFunction:InvokeClient()` or
`Class.RemoteFunction:InvokeServer()`. The code invoking the function
**yields** until it receives a response from the recipient.

In order for both the server and clients to access a `Class.RemoteFunction`
instance, it must be in a place where both sides can see it, such as
`Class.ReplicatedStorage`, although in some cases it's appropriate to store it
in `Class.Workspace` or inside a `Class.Tool`.

If the result is **not** needed, it is recommended that you use a
`Class.RemoteEvent` instead, since its call is asynchronous and doesn't need
to wait for a response to continue execution. See
[Remote Events and Callbacks](../../../scripting/events/remote.md) for code
samples and further details on `Class.RemoteFunction`.

#### Streaming Precautions

Note that if an invoked `Class.RemoteFunction` creates an instance on the
server, there is no guarantee that it exists on the client when the function
returns. This is particularly important in places where instance
[streaming](../../../workspace/streaming/index.md) is enabled and when the
created instances are `Class.BasePart|BaseParts` or `Class.Model|Models`,
since parts that are far away from the player's character may not be streamed
to the client, and models that are `Enum.ModelStreamingMode|Atomic` depend on
whether their parts are streamed. Even if a model is
`Enum.ModelStreamingMode|Persistent`, there may be some delay between the
creation of the model and when it is replicated to the client.

#### Parameter Limitations

Any type of Roblox object such as an `Datatype.Enum`, `Class.Instance`, or
others can be passed as a parameter when a `Class.RemoteFunction` is invoked,
as well as Luau types such as numbers, strings, and booleans, although you
should carefully explore the
[limitations](../../../scripting/events/remote.md#argument-limitations).

## Methods

### `Class.RemoteFunction:InvokeClient`

``InvokeClient(player: `Class.Player`, arguments: `Tuple`)`` -> `Tuple`
  [Yields]

### `Class.RemoteFunction:InvokeServer`

``InvokeServer(arguments: `Tuple`)`` -> `Tuple`
  [Yields]

## Callbacks

### `Class.RemoteFunction.OnClientInvoke`

``OnClientInvoke(arguments: `Tuple`)`` -> `Tuple`

### `Class.RemoteFunction.OnServerInvoke`

``OnServerInvoke(player: `Class.Player`, arguments: `Tuple`)`` -> `Tuple`

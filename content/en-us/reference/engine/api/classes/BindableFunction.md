---
title: BindableFunction
type: class
superclass: Instance
---

# BindableFunction

An object which allows for synchronous two-way communication between scripts
on the same side of the client-server boundary. Scripts invoking a
`Class.BindableFunction` yield until the corresponding callback is found.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

The **BindableFunction** object allows for synchronous two-way communication
between scripts on the same side of the
[client-server](../../../projects/client-server.md) boundary. You can use it
to define a custom callback function and invoke it manually by calling
`Class.BindableFunction:Invoke()`. The code invoking the function **yields**
until the corresponding callback is found, and the callback receives the
arguments that you passed to `Class.BindableFunction:Invoke()|Invoke()`. If
the callback was never set, the script that invokes it will not resume
execution.

As an alternative for one-way communication between two scripts on the same
side of the client-server boundary, consider `Class.BindableEvent` which does
**not** yield for a return.

As stated, `Class.BindableFunction|BindableFunctions` do not allow for
communication between the server and clients. If you are looking for this
functionality, use a `Class.RemoteFunction` as outlined in
[Remote events and callbacks](../../../scripting/events/remote.md).

See [Bindable events and callbacks](../../../scripting/events/bindable.md) for
code samples and further details on `Class.BindableFunction`.

#### Parameter Limitations

Any type of Roblox object such as an `Datatype.Enum`, `Class.Instance`, or
others can be passed as a parameter when a `Class.BindableFunction` is
invoked, as well as Luau types such as numbers, strings, and booleans,
although you should carefully explore the
[limitations](../../../scripting/events/bindable.md#argument-limitations).

## Methods

### `Class.BindableFunction:Invoke`

``Invoke(arguments: `Tuple`)`` -> `Tuple`
  [Yields]

## Callbacks

### `Class.BindableFunction.OnInvoke`

``OnInvoke(arguments: `Tuple`)`` -> `Tuple`

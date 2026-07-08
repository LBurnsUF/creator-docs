---
title: BindableEvent
type: class
superclass: Instance
---

# BindableEvent

An object which enables custom events through asynchronous one-way
communication between scripts on the same side of the client-server boundary.
Scripts firing a `Class.BindableEvent` do not yield.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

The **BindableEvent** object enables custom events through asynchronous
one-way communication between scripts on the same side of the
[client-server](../../../projects/client-server.md) boundary. When you fire a
`Class.BindableEvent` through the `Class.BindableEvent:Fire()` method, the
firing script does **not** yield and the target function receives the passed
arguments with certain [limitations](#argument-limitations).
`Class.BindableEvent|BindableEvents` create threads of each connected
function, so even if one firing errors, others continue.

As an alternative for two-way communication between two scripts on the same
side of the client-server boundary, consider `Class.BindableFunction`.

As stated, `Class.BindableEvent|BindableEvents` do not allow for communication
between the server and clients. If you are looking for this functionality, use
a `Class.RemoteEvent` as outlined in
[Remote Events and Callbacks](../../../scripting/events/remote.md).

See [Bindable events and callbacks](../../../scripting/events/bindable.md) for
code samples and further details on `Class.BindableEvent`.

#### Parameter Limitations

Any type of Roblox object such as an `Datatype.Enum`, `Class.Instance`, or
others can be passed as a parameter when a `Class.BindableEvent` is fired, as
well as Luau types such as numbers, strings, and booleans, although you should
carefully explore the
[limitations](../../../scripting/events/bindable.md#argument-limitations).

## Methods

### `Class.BindableEvent:Fire`

``Fire(arguments: `Tuple`)`` -> `null`

## Events

### `Class.BindableEvent.Event`

Fires with: (arguments: `Tuple`)

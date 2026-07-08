---
title: RBXScriptSignal
type: datatype
---

# `Datatype.RBXScriptSignal`

An object that runs connected functions upon a specific occurrence.

## Description

The `Datatype.RBXScriptSignal` data type, more commonly known as an **Event**,
provides a way for user-defined functions, called **listeners**, to call when
something happens in the game. When an event happens, the
`Datatype.RBXScriptSignal` fires and calls any listeners that are connected to
it. An `Datatype.RBXScriptSignal` may also pass arguments to each listener to
provide extra information about the event.

## Methods

### `RBXScriptSignal:Connect`

Establishes a function to be called when the event fires. Returns an
`Datatype.RBXScriptConnection` object associated with the connection.

**Parameters:**

- `func`: `function`

### `RBXScriptSignal:ConnectParallel`

Establishes a function to be called when the event fires. Returns an
`Datatype.RBXScriptConnection` object associated with the connection. When
the event fires, the signal callback is executed in a desynchronized
state. Using `ConnectParallel` is similar to, but more efficient than,
using `Connect` followed by a call to `Library.task.desynchronize()` in
the signal handler.

Note: Scripts that connect in parallel must be rooted under an Actor.

**Parameters:**

- `func`: `function`

### `RBXScriptSignal:Once`

Establishes a function to be called when the event fires. Returns an
`Datatype.RBXScriptConnection` object associated with the connection. The
behavior of `Once` is similar to `Connect`. However, instead of allowing
multiple events to be received by the specified function, only the first
event will be delivered. Using `Once` also ensures that the connection to
the function will be automatically disconnected prior the function being
called.

**Parameters:**

- `func`: `function`

### `RBXScriptSignal:Wait`

Yields the current thread until the signal fires and returns the arguments
provided by the signal.

## API Usage (15 locations)

### Used as Return Type

- `Class.AnimationTrack:GetMarkerReachedSignal`
- `Class.CollectionService:GetInstanceAddedSignal`
- `Class.CollectionService:GetInstanceRemovedSignal`
- `Class.ConfigSnapshot:GetValueChangedSignal`
- `Class.ContentProvider:GetAssetFetchStatusChangedSignal`
- `Class.Instance:GetAttributeChangedSignal`
- `Class.Instance:GetStyledPropertyChangedSignal`
- `Class.MaterialService:GetMaterialOverrideChanged`
- `Class.Object:GetPropertyChangedSignal`
- `Class.PlayerDataRecord:GetValueChangedSignal`
- `Class.RemoteCommandService:GetReceivedUpdateSignal`
- `Class.RemoteCommandService:GetStoppingSignal`
- `Class.TerrainIterateOperation:CommitBlock`
- `Class.TerrainModifyOperation:CommitBlock`
- `Class.TerrainWriteOperation:CommitBlock`

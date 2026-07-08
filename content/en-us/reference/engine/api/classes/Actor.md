---
title: Actor
type: class
superclass: Model
---

# Actor

An `Class.Actor` is a container for code that can be safely split into its own
thread.

**Inherits from:** `Class.Model` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

## Description

An `Class.Actor` is a container for code that can be safely split into its own
thread using `Library.task.desynchronize()`. It should also contain the
instances used by its scripts.

To learn more about using multiple Actors to optimize script performance, see
[Parallel Luau](../../../scripting/multithreading.md).

#### Notes

- Each `Actor` runs in its own Luau VM. `Class.ModuleScript|ModuleScripts`
  required by an `Actor` are **not** shared or cached across `Actors` or with
  the main thread. Each VM executes its own copy of the module, so
  module-level state is isolated per `Actor`. Design accordingly if your
  modules hold state you intend to share.
- `script:GetActor()` returns `nil` when called from a `Class.ModuleScript`
  unless the `ModuleScript` is a descendant of the `Actor`. `ModuleScripts`
  stored elsewhere (for example, `Class.ReplicatedStorage`) and required by an
  `Actor` are not considered descendants of the `Actor`.

## Methods

### `Class.Actor:BindToMessage`

``BindToMessage(topic: `string`, function: `Datatype.Function`)`` -> `Datatype.RBXScriptConnection`

### `Class.Actor:BindToMessageParallel`

``BindToMessageParallel(topic: `string`, function: `Datatype.Function`)`` -> `Datatype.RBXScriptConnection`

### `Class.Actor:SendMessage`

``SendMessage(topic: `string`, message: `Tuple`)`` -> `null`

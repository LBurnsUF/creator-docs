---
title: ProceduralModel
type: class
superclass: Model
---

# ProceduralModel

Procedural models support edit-time procedural generation. Instead of manually
constructing model content, a procedural model generates its contents
automatically in response to parameter changes.

**Inherits from:** `Class.Model` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

## Description

`ProceduralModel` inherits from `Class.Model` and supports edit-time
procedural generation of its contents. Instead of manually constructing model
content, a procedural model generates its contents automatically in response
to parameter changes.

Generation is defined by a **generator module**, a `Class.ModuleScript`
referenced by the `Class.ProceduralModel.Generator|Generator` property. The
engine invokes the module's `OnGenerate` function to produce the model's
contents.

A procedural model regenerates when any of the following inputs change:

- The `Class.ProceduralModel.Size|Size` property of the procedural model,
  which defines a bounding box for the model to generate within.
- Any attributes on the procedural mode, as defined by the generator module.
- The generator's module sandboxing configuration (`Sandboxed` and
  `Capabilities`).
- The source code of the generator module.

When any of these inputs change, the engine schedules regeneration. This
scheduled regeneration is performed by calling `OnGenerate` and applying its
results once it returns. In most cases, generation happens within the same
frame, but can be deferred to maintain performance.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ProceduralModel.GenerationError` | `string` | [ReadOnly] [NotReplicated] |
| `Class.ProceduralModel.Generator` | `Class.ModuleScript` |  |
| `Class.ProceduralModel.Size` | `Datatype.Vector3` |  |

## Methods

### `Class.ProceduralModel:ForceGeneration`

``ForceGeneration()`` -> `bool`

### `Class.ProceduralModel:WaitForGenerationAsync`

``WaitForGenerationAsync()`` -> `bool`
  [Yields]

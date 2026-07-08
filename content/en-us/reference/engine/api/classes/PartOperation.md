---
title: PartOperation
type: class
superclass: TriangleMeshPart
---

# PartOperation

An abstract class that all parts based on solid modeling inherit from.

**Inherits from:** `Class.TriangleMeshPart` > `Class.BasePart` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

## Description

An abstract class that all parts based on
[solid modeling](../../../parts/solid-modeling.md) inherit from.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.PartOperation.RenderFidelity` | `Enum.RenderFidelity` |  {write: PluginSecurity} |
| `Class.PartOperation.SmoothingAngle` | `float` |  {write: PluginSecurity} |
| `Class.PartOperation.TriangleCount` | `int` |  {write: RobloxSecurity} |
| `Class.PartOperation.UsePartColor` | `bool` |  |

## Methods

### `Class.PartOperation:SubstituteGeometry`

``SubstituteGeometry(source: `Class.Instance`)`` -> `null`

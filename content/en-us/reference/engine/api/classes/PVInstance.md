---
title: PVInstance
type: class
superclass: Instance
tags: [NotCreatable, NotBrowsable]
---

# PVInstance

Abstract class for all objects that have a physical location in the world.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotBrowsable]

## Description

A `Class.PVInstance` is an abstract class that cannot be created. It is the
base for all objects that have a physical location in the world.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.PVInstance.Origin` | `Datatype.CFrame` | [NotReplicated] [NotScriptable] |
| `Class.PVInstance.Pivot Offset` | `Datatype.CFrame` | [NotReplicated] [NotScriptable] |

## Methods

### `Class.PVInstance:GetPivot`

``GetPivot()`` -> `Datatype.CFrame`

### `Class.PVInstance:PivotTo`

``PivotTo(targetCFrame: `Datatype.CFrame`)`` -> `null`

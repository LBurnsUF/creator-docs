---
title: FloorWire
type: class
superclass: GuiBase3d
tags: [Deprecated]
---

# FloorWire

A FloorWire attempts to make a wire from two of its properties:
`Class.FloorWire.From` and `Class.FloorWire.From`, which both need to be set
to a `Class.BasePart`.

**Inherits from:** `Class.GuiBase3d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

**Tags:** [Deprecated]

## Description

A FloorWire attempts to make a wire from two of its properties:
`Class.FloorWire.From` and `Class.FloorWire.To`, which both need to be set to
a `Class.BasePart`. It sometimes goes through bricks but the majority of the
time it works fine. It starts at From's center and goes to To's center. Which
side of each one it goes into depends on the BaseParts's positions. It chooses
the fastest route.

> **Deprecated:** The FloorWire object has been deprecated and should not be used in new work.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.FloorWire.CycleOffset` | `float` |  |
| `Class.FloorWire.From` | `Class.BasePart` |  |
| `Class.FloorWire.StudsBetweenTextures` | `float` |  |
| `Class.FloorWire.Texture` | `Datatype.ContentId` |  |
| `Class.FloorWire.TextureSize` | `Datatype.Vector2` |  |
| `Class.FloorWire.To` | `Class.BasePart` |  |
| `Class.FloorWire.Velocity` | `float` |  |
| `Class.FloorWire.WireRadius` | `float` |  |

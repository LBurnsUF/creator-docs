---
title: SurfaceSelection
type: class
superclass: PartAdornment
---

# SurfaceSelection

Highlights a face of a surface in a configurable color.

**Inherits from:** `Class.PartAdornment` > `Class.GuiBase3d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Description

A `SurfaceSelection` highlights a particular face
(`Class.SurfaceSelection.TargetSurface|TargetSurface`) of its
`Class.PartAdornment.Adornee|Adornee`. The highlight's color is configurable
using the `Class.GuiBase3d.Color3|Color3` property.

The `SurfaceSelection` object is typically used by `Class.Plugin` when the
user is selecting the face of a `Class.BasePart`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.SurfaceSelection.TargetSurface` | `Enum.NormalId` |  |

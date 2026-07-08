---
title: SelectionSphere
type: class
superclass: PVAdornment
---

# SelectionSphere

Renders a 3D sphere around its `Class.PVAdornment.Adornee|Adornee`.

**Inherits from:** `Class.PVAdornment` > `Class.GuiBase3d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Description

`SelectionSphere` renders a 3D sphere around its
`Class.PVAdornment.Adornee|Adornee` when it is a descendant of the
`Class.Workspace` or anywhere where GUI objects are rendered. The sphere's
geometry consists of a ring/outline in addition to a surface.
`SelectionSphere` does not capture any form of input; it is solely a visual
effect.

For an outline/fill overlay effect which covers non‑primitive geometry such as
that of a `Class.MeshPart`, see `Class.Highlight`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.SelectionSphere.SurfaceColor` | `Datatype.BrickColor` | [Hidden] [NotReplicated] [Deprecated] |
| `Class.SelectionSphere.SurfaceColor3` | `Datatype.Color3` |  |
| `Class.SelectionSphere.SurfaceTransparency` | `float` |  |

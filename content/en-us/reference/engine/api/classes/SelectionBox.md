---
title: SelectionBox
type: class
superclass: InstanceAdornment
---

# SelectionBox

Renders a 3D box around its `Class.PVAdornment.Adornee|Adornee`.

**Inherits from:** `Class.InstanceAdornment` > `Class.GuiBase3d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Description

`SelectionBox` renders a 3D box around its `Class.PVAdornment.Adornee|Adornee`
when it is a descendant of the `Class.Workspace` or anywhere where GUI objects
are rendered. The box's geometry consists of rectangular prisms forming an
outline/wireframe in addition to a surface for each of its faces.
`SelectionBox` does not capture any form of input; it is solely a visual
effect.

For an outline/fill overlay effect which covers non‑primitive geometry such as
that of a `Class.MeshPart`, see `Class.Highlight`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.SelectionBox.LineThickness` | `float` |  |
| `Class.SelectionBox.StudioSelectionBox` | `bool` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.SelectionBox.SurfaceColor` | `Datatype.BrickColor` | [Hidden] [NotReplicated] [Deprecated] |
| `Class.SelectionBox.SurfaceColor3` | `Datatype.Color3` |  |
| `Class.SelectionBox.SurfaceTransparency` | `float` |  |

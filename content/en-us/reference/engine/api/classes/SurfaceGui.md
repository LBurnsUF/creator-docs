---
title: SurfaceGui
type: class
superclass: SurfaceGuiBase
---

# SurfaceGui

Container for GuiObjects that are rendered on the surface of a part.

**Inherits from:** `Class.SurfaceGuiBase` > `Class.LayerCollector` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Description

`Class.SurfaceGui` allows for the rendering of UI objects onto a part's
surface in the 3D world while also allowing for basic user interaction to
occur. Similar to `Class.Decal|Decals` and `Class.Texture|Textures`, UI
objects such as `Class.TextLabel|TextLabels` and
`Class.ImageLabel|ImageLabels` parented to a `Class.SurfaceGui` face the same
direction as the surface they're on, editable through the
`Class.SurfaceGui.Face|Face` property.

<img src="/assets/ui/in-experience/SurfaceGui-Diagram.jpg" width="800" alt="SurfaceGui on a 3D part in the place with an ImageLabel child to depict a screen console." />

Note that interactive UI elements like `Class.ImageButton|ImageButtons` and
`Class.TextButton|TextButtons` inside a `Class.SurfaceGui` will only receive
user input if they are parented to the `Class.PlayerGui`, typically via
placing the `Class.SurfaceGui` inside `Class.StarterGui` (the
`Class.SurfaceGui.Adornee|Adornee` property can be used to target a part in
the 3D world while the `Class.SurfaceGui` itself remains in the
`Class.PlayerGui`). Additionally, the part's
`Class.BasePart.CanQuery|CanQuery` property must be `true` for the interactive
UI element to receive input.

See [In-Experience UI](../../../ui/in-experience-containers.md#surface-ui) for
a guide on working with `Class.SurfaceGui` containers.

##### Caching Behavior

To help improve performance, the appearance of a `Class.SurfaceGui` is cached
until one of the following occurs, after which its appearance will be
recomputed on the next rendering frame.

- A descendant is added to or removed from the `Class.SurfaceGui`.
- A property of a descendant of the `Class.SurfaceGui` changes.
- A property of the `Class.SurfaceGui` itself changes.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.SurfaceGui.AlwaysOnTop` | `bool` |  |
| `Class.SurfaceGui.Brightness` | `float` |  |
| `Class.SurfaceGui.CanvasSize` | `Datatype.Vector2` |  |
| `Class.SurfaceGui.ClipsDescendants` | `bool` |  |
| `Class.SurfaceGui.HorizontalCurvature` | `float` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.SurfaceGui.LightInfluence` | `float` |  |
| `Class.SurfaceGui.MaxDistance` | `float` |  |
| `Class.SurfaceGui.PixelsPerStud` | `float` |  |
| `Class.SurfaceGui.Shape` | `Enum.SurfaceGuiShape` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.SurfaceGui.SizingMode` | `Enum.SurfaceGuiSizingMode` |  |
| `Class.SurfaceGui.ToolPunchThroughDistance` | `float` |  |
| `Class.SurfaceGui.ZOffset` | `float` |  |

---
title: BillboardGui
type: class
superclass: LayerCollector
---

# BillboardGui

A container for `Class.GuiObject|GuiObjects` that renders in 3D space facing
the camera.

**Inherits from:** `Class.LayerCollector` > `Class.GuiBase2d` > `Class.GuiBase` > `Class.Instance` > `Class.Object`

## Description

`Class.BillboardGui` is a container for UI objects to appear in the 3D space
but always face the camera. The container's position is relative to the parent
`Class.BasePart` or `Class.Attachment` (or the
`Class.BillboardGui.Adornee|Adornee`). For `Class.BasePart|BaseParts`, the
`Class.BasePart.Position|Position` property is used, while for
`Class.Attachment|Attachments`, the
`Class.Attachment.WorldPosition|WorldPosition` property is used.

<img src="/assets/ui/in-experience/BillboardGui-Diagram.jpg" width="800" alt="BillboardGui with a TextLabel describing the screen console it floats above." />

A billboard's `Class.BillboardGui.Size|Size` property works slightly
differently than `Class.GuiObject.Size`. While the **offset** components work
the same, the **scale** components are used as stud sizes in 3D space.

When creating a size-scaled `Class.BillboardGui` that contains a
`Class.TextLabel`, it's useful to enable the label's
`Class.TextLabel.TextScaled|TextScaled` property so that its text scales along
with the billboard canvas as the camera distance changes.

Note that interactive UI elements like `Class.ImageButton|ImageButtons` and
`Class.TextButton|TextButtons` inside a `Class.BillboardGui` will only receive
user input if they are parented to the `Class.PlayerGui`, typically via
placing the `Class.BillboardGui` inside `Class.StarterGui`. The
`Class.BillboardGui.Adornee|Adornee` property can be used to target a part or
attachment in the 3D world while the `Class.BillboardGui` itself remains in
the `Class.PlayerGui`.

See [In-Experience UI](../../../ui/in-experience-containers.md#billboard-ui)
for a guide on working with `Class.BillboardGui` containers.

##### Caching Behavior

To help improve performance, the appearance of a `Class.BillboardGui` is
cached until one of the following occurs, after which its appearance will be
recomputed on the next rendering frame.

- A descendant is added to or removed from the `Class.BillboardGui`.
- A property of a descendant of the `Class.BillboardGui` changes.
- A property of the `Class.BillboardGui` itself changes.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.BillboardGui.Active` | `bool` |  |
| `Class.BillboardGui.Adornee` | `Class.Instance` |  |
| `Class.BillboardGui.AlwaysOnTop` | `bool` |  |
| `Class.BillboardGui.Brightness` | `float` |  |
| `Class.BillboardGui.ClipsDescendants` | `bool` |  |
| `Class.BillboardGui.CurrentDistance` | `float` | [ReadOnly] [NotReplicated] |
| `Class.BillboardGui.DistanceLowerLimit` | `float` | [Deprecated] |
| `Class.BillboardGui.DistanceStep` | `float` | [NotReplicated] |
| `Class.BillboardGui.DistanceUpperLimit` | `float` | [Deprecated] |
| `Class.BillboardGui.ExtentsOffset` | `Datatype.Vector3` |  |
| `Class.BillboardGui.ExtentsOffsetWorldSpace` | `Datatype.Vector3` |  |
| `Class.BillboardGui.LightInfluence` | `float` |  |
| `Class.BillboardGui.MaxDistance` | `float` |  |
| `Class.BillboardGui.PlayerToHideFrom` | `Class.Instance` |  |
| `Class.BillboardGui.Size` | `Datatype.UDim2` |  |
| `Class.BillboardGui.SizeOffset` | `Datatype.Vector2` |  |
| `Class.BillboardGui.StudsOffset` | `Datatype.Vector3` |  |
| `Class.BillboardGui.StudsOffsetWorldSpace` | `Datatype.Vector3` |  |

## Methods

### `Class.BillboardGui:GetScreenSpaceBounds`

``GetScreenSpaceBounds()`` -> `Variant`
   {security: RobloxScriptSecurity}

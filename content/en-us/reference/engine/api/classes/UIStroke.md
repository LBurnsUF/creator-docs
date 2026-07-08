---
title: UIStroke
type: class
superclass: UIComponent
---

# UIStroke

Applies an outline to text or a UI border.

**Inherits from:** `Class.UIComponent` > `Class.UIBase` > `Class.Instance` > `Class.Object`

## Description

`Class.UIStroke` applies an outline to text or a UI border. Some properties
may require enabling the
[Improved UIStrokes beta](https://devforum.roblox.com/t/studio-beta-uistroke-improvements-scaling-offsets-and-more/3958036).

Key features include:

- Adjust the `Class.UIStroke.Color|Color` and
  `Class.UIStroke.Thickness|Thickness` of the stroke outline.
- Change the stroke `Class.UIStroke.Transparency|Transparency` independently
  from the text or UI object.
- Choose the `Class.UIStroke.LineJoinMode|LineJoinMode` of the stroke (round,
  bevel, or miter).
- Specify the `Class.UIStroke.BorderStrokePosition|BorderStrokePosition` on
  its parent's border and/or an additional
  `Class.UIStroke.BorderOffset|BorderOffset` to the stroke's position.
- Add a gradient to the stroke via the `Class.UIGradient` instance.
- Use [rich text](../../../ui/rich-text.md) tags to add stroke to inline text
  segments.

For more details on the `Class.UIStroke` object, see
[Appearance Modifiers](../../../ui/appearance-modifiers.md).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.UIStroke.ApplyStrokeMode` | `Enum.ApplyStrokeMode` |  |
| `Class.UIStroke.BorderOffset` | `Datatype.UDim` |  |
| `Class.UIStroke.BorderStrokePosition` | `Enum.BorderStrokePosition` |  |
| `Class.UIStroke.Color` | `Datatype.Color3` |  |
| `Class.UIStroke.Enabled` | `bool` |  |
| `Class.UIStroke.LineJoinMode` | `Enum.LineJoinMode` |  |
| `Class.UIStroke.StrokeSizingMode` | `Enum.StrokeSizingMode` |  |
| `Class.UIStroke.Thickness` | `float` |  |
| `Class.UIStroke.Transparency` | `float` |  |
| `Class.UIStroke.ZIndex` | `int` |  |

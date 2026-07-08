---
title: UIGradient
type: class
superclass: UIComponent
---

# UIGradient

Applies a color and transparency gradient to the UI elements rendered by the
parent `Class.GuiObject`.

**Inherits from:** `Class.UIComponent` > `Class.UIBase` > `Class.Instance` > `Class.Object`

## Description

**UIGradient** applies a color and transparency gradient to the UI elements
rendered by the parent `Class.GuiObject`. The appearance of the gradient is
configurable through its `Class.UIGradient.Color|Color`
(`Datatype.ColorSequence`), `Class.UIGradient.Transparency|Transparency`
(`Datatype.NumberSequence`), `Class.UIGradient.Offset|Offset`
(`Datatype.Vector2`), and `Class.UIGradient.Rotation|Rotation` (number).

A `Class.UIGradient` will not apply to child or descendant
`Class.GuiObject|GuiObjects`. In order to apply the same gradient to multiple
objects, you will need multiple gradient instances.

See also [Appearance Modifiers](../../../ui/appearance-modifiers.md) for more
information on `Class.UIGradient` objects and how they work.

#### Supported Objects

You can apply gradients to `Class.Frame`, `Class.TextLabel`,
`Class.TextButton`, `Class.ImageLabel`, `Class.ImageButton`, and
`Class.ViewportFrame`. However, `Class.ScrollingFrame` and `Class.TextBox` are
not currently supported.

#### Performance Considerations

In order to efficiently use a `Class.UIGradient`, follow these principles:

- Avoid using more than 6 color stops on the `Class.UIGradient.Color|Color`
  sequence.

- Avoid using a `Class.UIGradient` on any object that applies a text stroke
  (`Class.TextLabel.TextStrokeColor3|TextStrokeColor3`), as the gradient will
  try to blend with strokes and borders, and may cause performance issues.

- Avoid setting `Class.UIGradient.Color|Color` and
  `Class.UIGradient.Transparency|Transparency` frequently: this causes the
  sequence of colors to rebuild often, which is expensive. If possible, set
  these properties only once and try to animate the
  `Class.UIGradient.Offset|Offset` or `Class.UIGradient.Rotation|Rotation`
  properties to achieve a similar effect. Alternatively, you can change the
  color of the parent `Class.GuiObject` using such properties as
  `Class.GuiObject.BackgroundColor3|BackgroundColor3`,
  `Class.ImageLabel.ImageColor3|ImageColor3`, or
  `Class.TextLabel.TextColor3|TextColor3`.

- When applying an unchanging gradient on a UI element whose state changes a
  lot, there is a tradeoff between using a `Class.UIGradient` (processing
  time) and a static gradient image (memory).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.UIGradient.Color` | `Datatype.ColorSequence` |  |
| `Class.UIGradient.Enabled` | `bool` |  |
| `Class.UIGradient.Offset` | `Datatype.Vector2` |  |
| `Class.UIGradient.Rotation` | `float` |  |
| `Class.UIGradient.Scale` | `float` |  |
| `Class.UIGradient.TileMode` | `Enum.GradientTileMode` |  |
| `Class.UIGradient.Transparency` | `Datatype.NumberSequence` |  |
| `Class.UIGradient.Type` | `Enum.GradientType` |  |

---
title: UICorner
type: class
superclass: UIComponent
---

# UICorner

UI modifier which applies deformation to corners of its parent
`Class.GuiObject`.

**Inherits from:** `Class.UIComponent` > `Class.UIBase` > `Class.Instance` > `Class.Object`

## Description

`UICorner` is a modifier which applies deformation to corners of its parent
`Class.GuiObject`. Input, but not descendants, will be clipped to the round
corner area. See
[UI appearance modifiers](../../../ui/appearance-modifiers.md#corners) for
examples.

In order to keep the circular shape of round corners, each corner radius
(`Datatype.UDim`) is internally calculated as follows:

- The radius of the **X** axis is always the same as the radius of **Y** axis.
- `Datatype.UDim.Scale|Scale` rounding will always apply to the **minimum**
  width or height.
- Rounded rectangles will always be in a "pill" shape if
  `Class.UICorner.CornerRadius|CornerRadius` is set to a value that leads to a
  calculated result greater than half of the rectangle's minimum width or
  height.

Alternatively to `UICorner`, rounded corners can be accomplished using
**slices** which are suitable for decorative borders that are not simply
rounded. See [9‑Slice Design](../../../ui/9-slice.md) for details.

Note that `UICorner` can not be applied to a `Class.ScrollingFrame`.

#### Individual Corners

Each corner has its own radius property
(`Class.UICorner.TopLeftRadius|TopLeftRadius`,
`Class.UICorner.TopRightRadius|TopRightRadius`,
`Class.UICorner.BottomRightRadius|BottomRightRadius`,
`Class.UICorner.BottomLeftRadius|BottomLeftRadius`). The
`Class.UICorner.CornerRadius|CornerRadius` property is a convenience shorthand
that sets all four corners at once and reads from
`Class.UICorner.TopLeftRadius|TopLeftRadius`.

When using [styling](../../../ui/styling/index.md) with `UICorner`, avoid
configuring both `Class.UICorner.CornerRadius|CornerRadius` and the individual
corner radii in style rules at the same time, as this may produce unexpected
results.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.UICorner.BottomLeftRadius` | `Datatype.UDim` |  |
| `Class.UICorner.BottomRightRadius` | `Datatype.UDim` |  |
| `Class.UICorner.CornerRadius` | `Datatype.UDim` | [NotReplicated] |
| `Class.UICorner.TopLeftRadius` | `Datatype.UDim` |  |
| `Class.UICorner.TopRightRadius` | `Datatype.UDim` |  |

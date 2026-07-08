---
title: UIShadow
type: class
superclass: UIComponent
---

# UIShadow

Renders a shadow below the parent UI instance.

**Inherits from:** `Class.UIComponent` > `Class.UIBase` > `Class.Instance` > `Class.Object`

## Description

`UIShadow` renders a drop shadow below its parent UI instance. Key features
include:

- Adjust the shadow's bluriness with `Class.UIShadow.BlurRadius|BlurRadius`.
- Adjust the shadow's color and transparency with `Class.UIShadow.Color|Color`
  and `Class.UIShadow.Transparency|Transparency`.
- Adjust the shadow's position and size relative to the parent with
  `Class.UIShadow.Offset|Offset` and `Class.UIShadow.Spread|Spread`.
- Add multiple shadows under the same parent and adjust their render order
  with `Class.UIShadow.ZIndex|ZIndex`.
- If the parent is rotated with `Class.GuiObject.Rotation`, the shadow will
  also be rotated.
- If the parent has round corners with `Class.UICorner`, the shadow will also
  have round corners.

#### Limitations

- `UIShadow` does not support text. If you add a `UIShadow` to a
  `Class.TextLabel` or `Class.TextButton`, it renders a shadow of the object's
  rectangular bounding area, not of the text.
- `UIShadow` does not support inset shadows.
- `UIShadow` does not support `Class.Path2D`.
- You cannot apply textures or `Class.UIGradient|UIGradients` to a `UIShadow`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.UIShadow.BlurRadius` | `Datatype.UDim` |  |
| `Class.UIShadow.Color` | `Datatype.Color3` |  |
| `Class.UIShadow.Enabled` | `bool` |  |
| `Class.UIShadow.Offset` | `Datatype.UDim2` |  |
| `Class.UIShadow.Spread` | `Datatype.UDim2` |  |
| `Class.UIShadow.Transparency` | `float` |  |
| `Class.UIShadow.ZIndex` | `int` |  |

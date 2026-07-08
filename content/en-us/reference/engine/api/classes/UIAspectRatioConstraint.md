---
title: UIAspectRatioConstraint
type: class
superclass: UIConstraint
---

# UIAspectRatioConstraint

Ensures the parent UI element maintains a particular aspect ratio.

**Inherits from:** `Class.UIConstraint` > `Class.UIComponent` > `Class.UIBase` > `Class.Instance` > `Class.Object`

## Description

The `Class.UIAspectRatioConstraint` enforces a **width‑to‑height** aspect
ratio on a `Class.GuiObject` regardless of its core size, even if that size is
set as a percentage of its parent. For example, inserting this constraint as a
child of a `Class.Frame` and setting the constraint's
`Class.UIAspectRatioConstraint.AspectRatio|AspectRatio` property to `2`
(`2:1`) keeps the frame's width at twice that of its height. Similarly,
setting this constraint's
`Class.UIAspectRatioConstraint.AspectRatio|AspectRatio` property to `0.5`
(`0.5:1`) keeps the frame's width at half that of its height.

Setting this constraint's
`Class.UIAspectRatioConstraint.AspectRatio|AspectRatio` to the default of `1`
(`1:1`) is a convenient way to prevent non‑proportional scaling/stretching of
an `Class.ImageLabel` with a square image asset.

Note that when a UI object is under control of both a layout structure such as
`Class.UIListLayout` and a `Class.UIAspectRatioConstraint`, the constraint
will **override** the layout and control the object's size.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.UIAspectRatioConstraint.AspectRatio` | `float` |  |
| `Class.UIAspectRatioConstraint.AspectType` | `Enum.AspectType` |  |
| `Class.UIAspectRatioConstraint.DominantAxis` | `Enum.DominantAxis` |  |

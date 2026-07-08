---
title: UISizeConstraint
type: class
superclass: UIConstraint
---

# UISizeConstraint

Ensures a `Class.GuiObject` does not become larger or smaller than the
constraint's maximum size or minimum size.

**Inherits from:** `Class.UIConstraint` > `Class.UIComponent` > `Class.UIBase` > `Class.Instance` > `Class.Object`

## Description

The `Class.UISizeConstraint` ensures a `Class.GuiObject` does not become
larger or smaller than the `Class.UISizeConstraint.MaxSize|MaxSize` and
`Class.UISizeConstraint.MinSize|MinSize`. For example, if
`Class.UISizeConstraint.MaxSize|MaxSize` is set to
<Typography noWrap>`(200, 200)`</Typography> and
`Class.UISizeConstraint.MinSize|MinSize` to <Typography
noWrap>`(100, 100)`</Typography>, the constrained object cannot scale to be
larger than 200&times;200 pixels or smaller than 100&times;100 pixels.

Note that if the object with this constraint is also under the control of a
`Class.UILayout` such as `Class.UIGridLayout`, the **constraint** determines
the object's minimum/maximum size and overwrites any size the layout would
apply.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.UISizeConstraint.MaxSize` | `Datatype.Vector2` |  |
| `Class.UISizeConstraint.MinSize` | `Datatype.Vector2` |  |

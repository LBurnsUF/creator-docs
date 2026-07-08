---
title: UIGridLayout
type: class
superclass: UIGridStyleLayout
---

# UIGridLayout

Positions sibling UI elements by filling rows using the space of the parent UI
element.

**Inherits from:** `Class.UIGridStyleLayout` > `Class.UILayout` > `Class.UIComponent` > `Class.UIBase` > `Class.Instance` > `Class.Object`

## Description

A UIGridLayout (not to be confused with the abstract `Class.UIGridStyleLayout`
from which this class inherits) lays out sibling UI elements in multiple rows
within the parent UI element, adding elements to a row one-by-one until the
next element would not fit. It then continues adding elements in the next row.
A UIGridLayout will take UI elements' `Class.GuiObject.Size` and
`Class.GuiObject.Position` under control. While under control, these UI
elements' properties will not be editable in the Properties window.

By default, it lays out elements in **ascending** order where lower values
take more priority over higher values, but this can be changed to use
elements' names by changing `Class.UIListLayout.SortOrder` to **Name**. A
UIListLayout will automatically re-layout elements when elements are
added/removed, or if a relevant property changes:
`Class.GuiObject.LayoutOrder` or `Class.Instance.Name`. This can be triggered
manually by calling `Class.UIGridStyleLayout:ApplyLayout()`, though this is
typically not necessary.

The actual cell sizes are the same for all cells. A UIGridLayout will respect
UI constraints placed with it, such as `Class.UISizeConstraint` and
`Class.UIAspectRatioConstraint`. Elements in the layout can span multiple
cells if they have a `Class.UISizeConstraint` with a
`Class.UISizeConstraint.MinSize|MinSize` set higher than the
`Class.UIGridLayout.CellSize|CellSize`. It is possible to limit the number of
elements per row using `Class.UIGridLayout.FillDirectionMaxCells`. If set to
1, it is possible to create a single row of elements (as each element would be
positioned in its own row).

This layout is appropriate when line breaks are OK after arbitrary cells. For
example, a set of inventory spaces is a good use of this layout. If building a
table of values in which a line break is not appropriate in the middle of
tabular data, it might be a better idea to use a `Class.UITableLayout`
instead.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.UIGridLayout.AbsoluteCellCount` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] |
| `Class.UIGridLayout.AbsoluteCellSize` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] |
| `Class.UIGridLayout.CellPadding` | `Datatype.UDim2` |  |
| `Class.UIGridLayout.CellSize` | `Datatype.UDim2` |  |
| `Class.UIGridLayout.FillDirectionMaxCells` | `int` |  |
| `Class.UIGridLayout.StartCorner` | `Enum.StartCorner` |  |

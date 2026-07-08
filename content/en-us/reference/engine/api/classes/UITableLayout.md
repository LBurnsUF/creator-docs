---
title: UITableLayout
type: class
superclass: UIGridStyleLayout
---

# UITableLayout

Lays out sibling UI elements and their child UI elements as rows/columns and
cells in a table.

**Inherits from:** `Class.UIGridStyleLayout` > `Class.UILayout` > `Class.UIComponent` > `Class.UIBase` > `Class.Instance` > `Class.Object`

## Description

A UITableLayout lays out sibling UI elements as rows in a table. Child UI
elements (the table cells) of these rows are then arranged in columns (within
rows). Each cell within a row has the same height, and each cell within a
column has the same width.

By changing the `Class.UIGridStyleLayout.FillDirection`, sibling UI elements
can act as columns instead.

When applied, a UITableLayout will take control of sibling and cell elements'
`Class.GuiObject.Size` and `Class.GuiObject.Position`. Changing these in the
Properties window is still possible will not produce any effect.

Dimensions of the cells in the resulting table are controlled by the parent UI
element's dimensions. Unless `Class.UITableLayout.FillEmptySpaceColumns` or
`Class.UITableLayout.FillEmptySpaceRows` is enabled, the cell dimensions will
be that of the parent UI element (and thus tables with more than one cell
extend outside of their parent).

Cells will continue to respect `Class.UISizeConstraint` objects within them.
In other words, setting `Class.UISizeConstraint.MinSize` on
`Class.UISizeConstraint|UISizeConstraints` within the header cells can
determine the size of the rest of the cells. If
`Class.UISizeConstraint.MaxSize` restricts a cell's size from filling the
allotted space (i.e. another row/column is wider than it), it will align to
the top-left.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.UITableLayout.FillEmptySpaceColumns` | `bool` |  |
| `Class.UITableLayout.FillEmptySpaceRows` | `bool` |  |
| `Class.UITableLayout.MajorAxis` | `Enum.TableMajorAxis` |  |
| `Class.UITableLayout.Padding` | `Datatype.UDim2` |  |

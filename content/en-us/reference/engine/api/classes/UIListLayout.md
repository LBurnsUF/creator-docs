---
title: UIListLayout
type: class
superclass: UIGridStyleLayout
---

# UIListLayout

Positions sibling UI elements in rows or columns within the parent UI
container.

**Inherits from:** `Class.UIGridStyleLayout` > `Class.UILayout` > `Class.UIComponent` > `Class.UIBase` > `Class.Instance` > `Class.Object`

## Description

A `Class.UIListLayout` positions sibling UI elements in rows or columns within
the parent UI container, based on the
`Class.UIListLayout.FillDirection|FillDirection`. The
`Class.GuiObject.Position|Position` and `Class.GuiObject.Rotation|Rotation`
properties of each sibling `Class.GuiObject` are either ignored or overridden
by the list layout, while each sibling retains its defined
`Class.GuiObject.Size|Size` unless the layout is configured to utilize a flex
layout. See [List and Flex Layouts](../../../ui/list-flex-layouts.md) for
further information.

<img src="../../../assets/engine-api/classes/UIListLayout/FillDirection.png"
width="720" alt="UIListLayouts illustrating FillDirection of either horizontal
or vertical." />

To control the layout order of siblings, set
`Class.UIListLayout.SortOrder|SortOrder` to either `Enum.SortOrder.Name` or
`Enum.SortOrder.LayoutOrder`, then rename siblings in alphanumerical order or
set their `Class.GuiObject.LayoutOrder|LayoutOrder` value, respectively.
`Class.UIListLayout` will automatically re‑layout elements when elements are
added/removed, or if a sibling's `Class.Instance.Name|Name` or
`Class.GuiObject.LayoutOrder|LayoutOrder` changes.

<img src="../../../assets/engine-api/classes/UIListLayout/SortOrder.png"
width="720" alt="List layout examples illustrating numerical LayoutOrder
sorting or alphanumerical Name sorting." />

Padding between siblings is controlled through the
`Class.UIListLayout.Padding|Padding` property, and wrapping within the parent
container's bounds through the `Class.UIListLayout.Wraps|Wraps` boolean.
Alignment of siblings within the parent container is controlled through
`Class.UIListLayout.HorizontalAlignment|HorizontalAlignment` and
`Class.UIListLayout.VerticalAlignment|VerticalAlignment` unless the layout is
configured to utilize a
[flex layout](../../../ui/list-flex-layouts.md#flex-layouts).

Note that there are performance implications of using a
[flex‑enabled](../../../ui/list-flex-layouts.md#flex-layouts) list layout,
since extra calculations are needed to calculate flex basis sizes, flexed
sizes, and line wrapping. Flex is enabled on a `Class.UIListLayout` when the
following properties are set, or if any `Class.GuiObject` sibling has a
`Class.UIFlexItem` parented to it:

- `Class.UIListLayout.HorizontalFlex|HorizontalFlex` and/or
  `Class.UIListLayout.VerticalFlex|VerticalFlex` are **not** set to
  `Enum.UIFlexAlignment.None`.
- `Class.UIListLayout.ItemLineAlignment|ItemLineAlignment` is **not** set to
  `Enum.ItemLineAlignment.Automatic`.
- `Class.UIListLayout.Wraps|Wraps` is `true`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.UIListLayout.HorizontalFlex` | `Enum.UIFlexAlignment` |  |
| `Class.UIListLayout.ItemLineAlignment` | `Enum.ItemLineAlignment` |  |
| `Class.UIListLayout.Padding` | `Datatype.UDim` |  |
| `Class.UIListLayout.VerticalFlex` | `Enum.UIFlexAlignment` |  |
| `Class.UIListLayout.Wraps` | `bool` |  |

---
title: ItemLineAlignment
type: enum
---

# `Enum.ItemLineAlignment`

Used for `Class.UIListLayout.ItemLineAlignment` and
`Class.UIFlexItem.ItemLineAlignment` in a flex layout to define the
cross-directional alignment of siblings or the parent within a line.

In a [flex layout](../../../ui/list-flex-layouts.md#flex-layouts), this enum
is used for the `Class.UIListLayout.ItemLineAlignment|ItemLineAlignment`
property of the `Class.UIListLayout` to define the **cross-directional**
alignment of siblings within a line. It is also used for the
`Class.UIFlexItem.ItemLineAlignment|ItemLineAlignment` property of a specific
`Class.UIFlexItem` to define the cross-directional alignment of the parent
`Class.GuiObject` within the line.

<img
src="../../../assets/engine-api/classes/UIListLayout/ItemLineAlignment.png"
width="720" alt="Examples of options for ItemLineAlignment in a horizontal
fill direction." />

The `Enum.ItemLineAlignment` enum has 5 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ItemLineAlignment.Automatic` | 0 | Aligns the siblings of the `Class.UIListLayout` or the specific `Class.UIFlexItem` parent to the lay |
| `Enum.ItemLineAlignment.Start` | 1 | Aligns the siblings of the `Class.UIListLayout` or the specific `Class.UIFlexItem` parent to the lin |
| `Enum.ItemLineAlignment.Center` | 2 | Aligns the siblings of the `Class.UIListLayout` or the specific `Class.UIFlexItem` parent to the lin |
| `Enum.ItemLineAlignment.End` | 3 | Aligns the siblings of the `Class.UIListLayout` or the specific `Class.UIFlexItem` parent to the lin |
| `Enum.ItemLineAlignment.Stretch` | 4 | Stretches the siblings of the `Class.UIListLayout` or the specific `Class.UIFlexItem` parent to fill |

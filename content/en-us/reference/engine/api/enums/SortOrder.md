---
title: SortOrder
type: enum
---

# `Enum.SortOrder`

Used by `Class.UIGridStyleLayout.SortOrder` to order the elements in the
layout.

Used by `Class.UIGridStyleLayout.SortOrder` to order the elements in the
layout.

<img src="../../../assets/engine-api/classes/UIListLayout/SortOrder.png" width="720" />

The `Enum.SortOrder` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.SortOrder.Name` | 0 | Elements are ordered by their `Class.Instance.Name` in alphanumeric order. |
| `Enum.SortOrder.Custom` | 1 | Elements are ordered by the function passed to `Class.UIGridStyleLayout:SetCustomSortFunction()`. |
| `Enum.SortOrder.LayoutOrder` | 2 | Elements are ordered by `Class.GuiObject.LayoutOrder` in ascending order; for example `0` will be pl |

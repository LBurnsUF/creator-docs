---
title: AutomaticSize
type: enum
---

# `Enum.AutomaticSize`

UI objects with `Class.GuiObject.AutomaticSize|AutomaticSize` enabled will
increase in size up to maximum size allowed by the parent (if there is one)
and no smaller than the `Class.GuiObject.Size|Size` property bounds.

UI objects with `Class.GuiObject.AutomaticSize|AutomaticSize` enabled will
increase in size up to maximum size allowed by the parent (if there is one)
and no smaller than the `Class.GuiObject.Size|Size` property bounds. To enable
`Enum.AutomaticSize`, set the value to an enum value other than `None`.

This enum is used by `Class.GuiObject.AutomaticSize` and
`Class.ScrollingFrame.AutomaticCanvasSize` to determine whether and how
resizing occurs based on child content.

For more information, see
[Automatic Sizing](../../../ui/size-modifiers.md#automatic-sizing).

The `Enum.AutomaticSize` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.AutomaticSize.None` | 0 | Default sizing behavior. |
| `Enum.AutomaticSize.X` | 1 | Automatically resize element along the **X** axis to fit child contents. |
| `Enum.AutomaticSize.Y` | 2 | Automatically resize element along the **Y** axis to fit child contents. Text objects will only resi |
| `Enum.AutomaticSize.XY` | 3 | Automatically resize element along the **X** and **Y** axes to fit child contents. |

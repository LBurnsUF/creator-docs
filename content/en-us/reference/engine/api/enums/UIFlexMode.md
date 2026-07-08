---
title: UIFlexMode
type: enum
---

# `Enum.UIFlexMode`

Used with `Class.UIFlexItem.FlexMode` to define how the parent
`Class.GuiObject` grows or shrinks.

Used with `Class.UIFlexItem.FlexMode` to define how the parent
`Class.GuiObject` grows or shrinks with available space in the container.

The `Enum.UIFlexMode` enum has 5 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.UIFlexMode.None` | 0 | The parent `Class.GuiObject` is unaffected and neither shrinks nor grows. |
| `Enum.UIFlexMode.Grow` | 1 | Sets an effective `1:0` grow‑shrink ratio on the parent `Class.GuiObject`. Objects set to `Grow` nev |
| `Enum.UIFlexMode.Shrink` | 2 | Sets an effective `0:1` grow‑shrink ratio on the parent `Class.GuiObject`. Objects set to `Shrink` n |
| `Enum.UIFlexMode.Fill` | 3 | Sets an effective `1:1` grow‑shrink ratio on the parent `Class.GuiObject`. This setting ensures the  |
| `Enum.UIFlexMode.Custom` | 4 | Enables the `Class.UIFlexItem.GrowRatio/GrowRatio` and `Class.UIFlexItem.ShrinkRatio/ShrinkRatio` pr |

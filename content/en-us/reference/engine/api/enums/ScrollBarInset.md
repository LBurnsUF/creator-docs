---
title: ScrollBarInset
type: enum
---

# `Enum.ScrollBarInset`

This enum is used with `Class.ScrollingFrame.HorizontalScrollBarInset` and
`Class.ScrollingFrame.VerticalScrollBarInset` to indicate whether the canvas
should be inset by
`Class.ScrollingFrame.ScrollBarThickness|ScrollBarThickness` for the
respective scroll bar.

This enum is used with `Class.ScrollingFrame.HorizontalScrollBarInset` and
`Class.ScrollingFrame.VerticalScrollBarInset` to indicate whether the canvas
should be inset by
`Class.ScrollingFrame.ScrollBarThickness|ScrollBarThickness` for the
respective scroll bar.

The `Enum.ScrollBarInset` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ScrollBarInset.None` | 0 | The canvas will never be inset for the respective scroll bar. |
| `Enum.ScrollBarInset.ScrollBar` | 1 | The canvas will only be inset if the respective scroll bar is showing. |
| `Enum.ScrollBarInset.Always` | 2 | The canvas will always be inset for the respective scroll bar, regardless of whether that scroll bar |

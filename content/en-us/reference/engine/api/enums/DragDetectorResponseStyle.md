---
title: DragDetectorResponseStyle
type: enum
---

# `Enum.DragDetectorResponseStyle`

Describes how the clicked object will be treated once the desired motion has
been calculated.

Describes how the clicked object will be treated once the desired motion has
been calculated.

The `Enum.DragDetectorResponseStyle` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.DragDetectorResponseStyle.Geometric` | 0 | For an `Class.BasePart.Anchored/Anchored` object both inside the running experience and in Studio ed |
| `Enum.DragDetectorResponseStyle.Physical` | 1 | An `Class.BasePart.Anchored/Anchored` object will default to **Geometric** behavior as it is not aff |
| `Enum.DragDetectorResponseStyle.Custom` | 2 | The object will not move at all, but `Class.DragDetector.DragFrame/DragFrame` will still be updated  |

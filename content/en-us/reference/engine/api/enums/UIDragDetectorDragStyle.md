---
title: UIDragDetectorDragStyle
type: enum
---

# `Enum.UIDragDetectorDragStyle`

Used with `Class.UIDragDetector` as the paradigm to generate proposed motion,
given a stream of input position vectors.

Used with `Class.UIDragDetector` as the paradigm to generate proposed motion,
given a stream of input position vectors.

The `Enum.UIDragDetectorDragStyle` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.UIDragDetectorDragStyle.TranslatePlane` | 0 | 2D motion in the plane of the `Class.LayerCollector`. |
| `Enum.UIDragDetectorDragStyle.TranslateLine` | 1 | 1D motion along the detector's `Class.UIDragDetector.DragAxis/DragAxis`. |
| `Enum.UIDragDetectorDragStyle.Rotate` | 2 | By default, rotation about the absolute center position of the detector's parent `Class.GuiObject`.  |
| `Enum.UIDragDetectorDragStyle.Scriptable` | 3 | Calculates desired motion via a custom function provided through `Class.UIDragDetector:SetDragStyleF |

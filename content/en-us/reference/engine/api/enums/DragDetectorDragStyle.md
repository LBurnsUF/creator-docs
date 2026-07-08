---
title: DragDetectorDragStyle
type: enum
---

# `Enum.DragDetectorDragStyle`

Used with `Class.DragDetector` as the paradigm to generate proposed motion,
given a stream of cursor rays.

Used with `Class.DragDetector` as the paradigm to generate proposed motion,
given a stream of cursor rays.

The `Enum.DragDetectorDragStyle` enum has 9 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.DragDetectorDragStyle.TranslateLine` | 0 | 1D motion along the detector's `Class.DragDetector.Axis/Axis`, by default the world **Y** axis. |
| `Enum.DragDetectorDragStyle.TranslatePlane` | 1 | 2D motion in the plane **perpendicular** to the detector's `Class.DragDetector.Axis/Axis`, by defaul |
| `Enum.DragDetectorDragStyle.TranslatePlaneOrLine` | 2 | 2D motion in the plane **perpendicular** to the detector's `Class.DragDetector.Axis/Axis` and, when  |
| `Enum.DragDetectorDragStyle.TranslateLineOrPlane` | 3 | 1D motion along the detector's `Class.DragDetector.Axis/Axis` and, when the modifier is active, 2D m |
| `Enum.DragDetectorDragStyle.TranslateViewPlane` | 4 | 2D motion in the plane perpendicular to the camera's view. In this mode, the plane is constantly upd |
| `Enum.DragDetectorDragStyle.RotateAxis` | 5 | Rotation about the detector's `Class.DragDetector.Axis/Axis`, by default the world **Y** axis. |
| `Enum.DragDetectorDragStyle.RotateTrackball` | 6 | Trackball rotation, further customized through the `Class.DragDetector.TrackballRadialPullFactor/Tra |
| `Enum.DragDetectorDragStyle.Scriptable` | 7 | Calculates desired motion via a custom function provided through `Class.DragDetector:SetDragStyleFun |
| `Enum.DragDetectorDragStyle.BestForDevice` | 8 | **TranslatePlaneOrLine** for mouse and gamepad; **TranslatePlane** for touch; **6DOF** for VR. |

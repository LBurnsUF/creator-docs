---
title: UIDragDetectorBoundingBehavior
type: enum
---

# `Enum.UIDragDetectorBoundingBehavior`

Used with `Class.UIDragDetector` to determine bounding behavior of the dragged
UI object when `Class.UIDragDetector.BoundingUI` is set.

Used with `Class.UIDragDetector` to determine bounding behavior of the dragged
UI object when `Class.UIDragDetector.BoundingUI` is set.

The `Enum.UIDragDetectorBoundingBehavior` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.UIDragDetectorBoundingBehavior.Automatic` | 0 | Mimics **EntireObject** behavior for a UI object that's entirely contained by the `Class.UIDragDetec |
| `Enum.UIDragDetectorBoundingBehavior.EntireObject` | 1 | Bounds the entire dragged UI object within the `Class.UIDragDetector.BoundingUI/BoundingUI`. |
| `Enum.UIDragDetectorBoundingBehavior.HitPoint` | 2 | Bounds the dragged UI only by the exact hit/grab point and its respective position after translation |

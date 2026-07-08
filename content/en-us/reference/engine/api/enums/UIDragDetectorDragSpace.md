---
title: UIDragDetectorDragSpace
type: enum
---

# `Enum.UIDragDetectorDragSpace`

Used with `Class.DragDetector` to set the paradigm which defines the space of
inputs/outputs from a custom drag function.

Used with `Class.DragDetector` to set the paradigm which defines the space of
inputs/outputs from a custom drag function registered through
`Class.UIDragDetector:SetDragStyleFunction()|SetDragStyleFunction()` or
`Class.UIDragDetector:AddConstraintFunction()|AddConstraintFunction()`.

The `Enum.UIDragDetectorDragSpace` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.UIDragDetectorDragSpace.Parent` | 0 | Designates the input and return values' space as the local space of the detector's parent `Class.Gui |
| `Enum.UIDragDetectorDragSpace.LayerCollector` | 1 | Designates the input and return values' space as that of the `Class.LayerCollector`. |
| `Enum.UIDragDetectorDragSpace.Reference` | 2 | Designates the input and return values' space as that of the `Class.UIDragDetector.ReferenceUIInstan |

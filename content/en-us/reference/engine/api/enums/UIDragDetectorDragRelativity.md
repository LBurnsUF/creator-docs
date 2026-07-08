---
title: UIDragDetectorDragRelativity
type: enum
---

# `Enum.UIDragDetectorDragRelativity`

Used with `Class.DragDetector` to set the paradigm which defines the
relativity of inputs/outputs from a custom drag function.

Used with `Class.DragDetector` to set the paradigm which defines the
relativity of inputs/outputs from a custom drag function registered through
`Class.UIDragDetector:SetDragStyleFunction()|SetDragStyleFunction()` or
`Class.UIDragDetector:AddConstraintFunction()|AddConstraintFunction()`.

The `Enum.UIDragDetectorDragRelativity` enum has 2 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.UIDragDetectorDragRelativity.Absolute` | 0 | Designates the input and return values as the absolute target position/rotation in the space defined |
| `Enum.UIDragDetectorDragRelativity.Relative` | 1 | Designates the input and return values as the change from the current position/rotation in the space |

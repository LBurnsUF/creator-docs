---
title: AlignType
type: enum
---

# `Enum.AlignType`

An enum that specifies how the constraint will attempt to align the body
associated with the constraint.

An enum that specifies how the constraint will attempt to align the body
associated with the constraint and attachment. Depending on the configuration,
it can be used to align specific axes to be parallel, perpendicular, or to
look at a specific point.

The `Enum.AlignType` enum has 6 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.AlignType.Parallel` | 0 |  |
| `Enum.AlignType.Perpendicular` | 1 |  |
| `Enum.AlignType.PrimaryAxisParallel` | 2 | Aligns the primary axis to be parallel to the axis given by `Class.Constraint.Attachment1`. |
| `Enum.AlignType.PrimaryAxisPerpendicular` | 3 | Aligns the primary axis to be perpendicular to the axis given by `Class.Constraint.Attachment1`. |
| `Enum.AlignType.PrimaryAxisLookAt` | 4 | Aligns the primary axis to look at the point given by `Class.Constraint.Attachment1` or the `Class.A |
| `Enum.AlignType.AllAxes` | 5 | Aligns all of the axes of `Class.Constraint.Attachment0` to the axes given by `Class.Constraint.Atta |

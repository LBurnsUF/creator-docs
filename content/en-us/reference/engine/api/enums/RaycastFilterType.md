---
title: RaycastFilterType
type: enum
---

# `Enum.RaycastFilterType`

Used in a `Datatype.RaycastParams` object to determine how its
`Datatype.RaycastParams.FilterDescendantsInstances|FilterDescendantsInstances`
list will be used.

Used in a `Datatype.RaycastParams` object to determine how its
`Datatype.RaycastParams.FilterDescendantsInstances|FilterDescendantsInstances`
list will be used.

The `Enum.RaycastFilterType` enum has 2 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.RaycastFilterType.Exclude` | 0 | Every `Class.BasePart` in the raycast operation will be considered **except** those that are descend |
| `Enum.RaycastFilterType.Include` | 1 | Only `Class.BasePart/BaseParts` which are descendants of objects in the filter list will be consider |

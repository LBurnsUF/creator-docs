---
title: VelocityConstraintMode
type: enum
---

# `Enum.VelocityConstraintMode`

The velocity constraint mode property controls how the linear velocity of the
attachment(s) is constrained.

The velocity constraint mode sets how the attachment velocity is constrained.
The velocity can be constrained to a line, a plane or a vector. See each mode
for more details.

The `Enum.VelocityConstraintMode` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.VelocityConstraintMode.Line` | 0 | The velocity component in the direction of the line is constrained to the specified value. The line  |
| `Enum.VelocityConstraintMode.Plane` | 1 | The velocity components in the plane are constrained to the specified values. The plane tangents are |
| `Enum.VelocityConstraintMode.Vector` | 2 | The velocity components must be equal to the vector components specified. The coordinate system of t |

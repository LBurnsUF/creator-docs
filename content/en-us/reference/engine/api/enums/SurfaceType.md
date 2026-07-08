---
title: SurfaceType
type: enum
---

# `Enum.SurfaceType`

Used to determine how a surface should be displayed on a part and how
automatic surface joints should behave.

Used to determine how a surface should be displayed on a part and how
automatic surface joints should behave.

The `Enum.SurfaceType` enum has 10 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.SurfaceType.Smooth` | 0 | Adds no details on the surface. |
| `Enum.SurfaceType.Glue` | 1 | Adds an "X" pattern across the surface. |
| `Enum.SurfaceType.Weld` | 2 | Adds an "X" pattern across the surface. |
| `Enum.SurfaceType.Studs` | 3 | Adds square studs across the surface. |
| `Enum.SurfaceType.Inlet` | 4 | Adds square holes across the surface where studs would be. |
| `Enum.SurfaceType.Universal` | 5 | Adds a checker pattern to the surface using studs and inlets. |
| `Enum.SurfaceType.Hinge` | 6 | Adds a yellow hinge to the surface. Parts touching it stick to the surface, allowing for rotations u |
| `Enum.SurfaceType.Motor` | 7 | Functioned identically to a hinge with the addition of a grey ring. |
| `Enum.SurfaceType.SteppingMotor` | 8 | Functioned identically to a motor. It may have functioned differently in the past, but that function |
| `Enum.SurfaceType.SmoothNoOutlines` | 10 | Previously similar to **Smooth** with outlines but no longer relevant since outlines have been remov |

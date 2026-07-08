---
title: SurfaceLight
type: class
superclass: Light
---

# SurfaceLight

A light source that emits illumination of a specified color and brightness
from a face for a specified range.

**Inherits from:** `Class.Light` > `Class.Instance` > `Class.Object`

## Description

A SurfaceLight is a light source that emits illumination of a specified
`Class.Light.Color` and `Class.Light.Brightness` from a
`Class.SurfaceLight.Face` for a specified `Class.SurfaceLight.Range`.

In order for a SurfaceLight to provide illumination, it must be the direct
child of a `Class.BasePart` or `Class.Attachment` (the part or attachment
itself must be a descendant of the Workspace). If a SurfaceLight is parented
to a part, then the light will emanate from the part's selected face(s). If
parented to an attachment SurfaceLight is equivalent to a `Class.SpotLight`.

For more light types, please see the **see also** section.

## See Also

- `Class.PointLight`
- `Class.SpotLight`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.SurfaceLight.Angle` | `float` |  |
| `Class.SurfaceLight.Face` | `Enum.NormalId` |  |
| `Class.SurfaceLight.Range` | `float` |  |

---
title: PointLight
type: class
superclass: Light
---

# PointLight

A light source that emits illumination from a single point.

**Inherits from:** `Class.Light` > `Class.Instance` > `Class.Object`

## Description

A PointLight is a light source that emits illumination from a single point.
Light is emitted spherically based on the `Class.PointLight.Range` of the
PointLight.

In order for a PointLight to provide illumination, it must be the direct child
of a `Class.BasePart` or `Class.Attachment` (the part or attachment itself
must be a descendant of the `Class.Workspace`).

If a PointLight is parented to a part, then the light will emanate from the
part's `Class.BasePart.Position`. If a PointLight is parented to an
attachment, then the light will emanate from the attachment's
`Class.Attachment.WorldPosition`.

For more light types, see the **see also** section.

## See Also

- `Class.SurfaceLight`
- `Class.SpotLight`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.PointLight.Range` | `float` |  |

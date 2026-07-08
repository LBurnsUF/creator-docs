---
title: SpotLight
type: class
superclass: Light
---

# SpotLight

A light source that emits light directionally in the shape of a cone with a
spherical base.

**Inherits from:** `Class.Light` > `Class.Instance` > `Class.Object`

## Description

A **Spotlight** emits light of a specified `Class.Light.Color|Color` and
`Class.Light.Brightness|Brightness` in the shape of a cone with a spherical
base. This object is ideal for **directional** light sources like flashlights
and headlights.

`Class.SpotLight.Range|Range` controls the distance of illumination and
`Class.SpotLight.Angle|Angle` defines the angle of light emission from the
cone's apex as illustrated below.

A spotlight must be a direct child of a `Class.BasePart` or `Class.Attachment`
and will exhibit the following behavior:

- When the spotlight is parented to a `Class.BasePart`, the
  `Class.SpotLight.Face|Face` property determines the face of the part from
  which light emanates.

- Although `Class.Attachment|Attachments` don't have faces, the
  `Class.SpotLight.Face|Face` property determines the axis of the attachment
  from which light emanates; **-Z** is front, **+X** is right, **+Y** is top,
  etc.

See also `Class.SurfaceLight` and `Class.PointLight`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.SpotLight.Angle` | `float` |  |
| `Class.SpotLight.Face` | `Enum.NormalId` |  |
| `Class.SpotLight.Range` | `float` |  |

---
title: Sky
type: class
superclass: Instance
---

# Sky

Changes the default appearance of the experience's sky.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

The `Sky` object, when placed inside `Class.Lighting`, changes the default
appearance of the experience's sky. This object's
[skybox](../../../environment/skybox.md) is composed of six sides, like a
cube. Rotation of the skybox can be changed through
`Class.Sky.SkyboxOrientation|SkyboxOrientation`.

The skybox sun, moon, and other celestial objects remain visible unless you
turn off the `Class.Sky.CelestialBodiesShown|CelestialBodiesShown` property.
By adjusting the `Class.Sky.StarCount|StarCount` property, you can change how
many stars appear in the sky at night.

This object can also be used as a cubemap for reflections in
`Class.ViewportFrame|ViewportFrames`, in which case only the `Class.Sky`
object's six‑side `Skybox[…]` properties are used. For details, see
[viewport frames](../../../ui/viewport-frames.md).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Sky.CelestialBodiesShown` | `bool` |  |
| `Class.Sky.MoonAngularSize` | `float` |  |
| `Class.Sky.MoonTextureContent` | `Datatype.Content` |  |
| `Class.Sky.MoonTextureId` | `Datatype.ContentId` |  |
| `Class.Sky.SkyboxBackContent` | `Datatype.Content` |  |
| `Class.Sky.SkyboxBk` | `Datatype.ContentId` |  |
| `Class.Sky.SkyboxDn` | `Datatype.ContentId` |  |
| `Class.Sky.SkyboxDownContent` | `Datatype.Content` |  |
| `Class.Sky.SkyboxFrontContent` | `Datatype.Content` |  |
| `Class.Sky.SkyboxFt` | `Datatype.ContentId` |  |
| `Class.Sky.SkyboxLeftContent` | `Datatype.Content` |  |
| `Class.Sky.SkyboxLf` | `Datatype.ContentId` |  |
| `Class.Sky.SkyboxOrientation` | `Datatype.Vector3` |  |
| `Class.Sky.SkyboxRightContent` | `Datatype.Content` |  |
| `Class.Sky.SkyboxRt` | `Datatype.ContentId` |  |
| `Class.Sky.SkyboxUp` | `Datatype.ContentId` |  |
| `Class.Sky.SkyboxUpContent` | `Datatype.Content` |  |
| `Class.Sky.StarCount` | `int` |  |
| `Class.Sky.SunAngularSize` | `float` |  |
| `Class.Sky.SunTextureContent` | `Datatype.Content` |  |
| `Class.Sky.SunTextureId` | `Datatype.ContentId` |  |

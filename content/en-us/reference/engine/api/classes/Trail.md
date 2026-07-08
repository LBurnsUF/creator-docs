---
title: Trail
type: class
superclass: Instance
---

# Trail

Used to create a trail effect between two attachments.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

The **Trail** object is used to create a trail effect between two attachments.
As the attachments move through space, a texture is drawn on their defined
plane. This is commonly used to create effects that visualize movements like
tracer trails behind projectiles, footprints, tire tracks, and similar
effects.

See [Trails](../../../effects/trails.md) for more information.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Trail.Attachment0` | `Class.Attachment` |  |
| `Class.Trail.Attachment1` | `Class.Attachment` |  |
| `Class.Trail.Brightness` | `float` |  |
| `Class.Trail.Color` | `Datatype.ColorSequence` |  |
| `Class.Trail.Enabled` | `bool` |  |
| `Class.Trail.FaceCamera` | `bool` |  |
| `Class.Trail.Lifetime` | `float` |  |
| `Class.Trail.LightEmission` | `float` |  |
| `Class.Trail.LightInfluence` | `float` |  |
| `Class.Trail.LocalTransparencyModifier` | `float` | [Hidden] [NotReplicated] |
| `Class.Trail.MaxLength` | `float` |  |
| `Class.Trail.MinLength` | `float` |  |
| `Class.Trail.Texture` | `Datatype.ContentId` |  |
| `Class.Trail.TextureContent` | `Datatype.Content` |  |
| `Class.Trail.TextureLength` | `float` |  |
| `Class.Trail.TextureMode` | `Enum.TextureMode` |  |
| `Class.Trail.Transparency` | `Datatype.NumberSequence` |  |
| `Class.Trail.WidthScale` | `Datatype.NumberSequence` |  |

## Methods

### `Class.Trail:Clear`

``Clear()`` -> `null`

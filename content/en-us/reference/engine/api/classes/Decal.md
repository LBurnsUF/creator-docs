---
title: Decal
type: class
superclass: FaceInstance
---

# Decal

Applies an image texture to a face of a parent `Class.BasePart`.

**Inherits from:** `Class.FaceInstance` > `Class.Instance` > `Class.Object`

## Description

The `Class.Decal` object applies an image texture to a face of a parent
`Class.BasePart`. The affected face is dependent on the
`Class.Decal.Face|Face` property, and the size of the decal is dependent on
the size of the face.

The applied image texture is determined by its
`Class.Decal.ColorMapContent|ColorMapContent` property. For details on how to
upload images, see
[asset management](../../../projects/assets/index.md#asset-management).

For more information, review
[textures and decals](../../../parts/textures-decals.md). See also:

- `Class.Texture` for repeating surface images.
- `Class.MeshPart.TextureContent` to apply an image texture to a
  `Class.MeshPart`.
- `Class.SurfaceGui` to apply an `Class.ImageLabel` or `Class.ImageButton` to
  an in-experience 3D object.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Decal.AutoLocalize` | `bool` |  |
| `Class.Decal.Color3` | `Datatype.Color3` |  |
| `Class.Decal.ColorMap` | `Datatype.ContentId` | [NotReplicated] |
| `Class.Decal.ColorMapContent` | `Datatype.Content` | [NotReplicated] |
| `Class.Decal.LocalTransparencyModifier` | `float` | [Hidden] [NotReplicated] |
| `Class.Decal.MetalnessMap` | `Datatype.ContentId` | [Hidden] {security: PluginSecurity} |
| `Class.Decal.MetalnessMapContent` | `Datatype.Content` |  {write: PluginSecurity} |
| `Class.Decal.NormalMap` | `Datatype.ContentId` | [Hidden] {security: PluginSecurity} |
| `Class.Decal.NormalMapContent` | `Datatype.Content` |  {write: PluginSecurity} |
| `Class.Decal.Rotation` | `float` |  |
| `Class.Decal.RoughnessMap` | `Datatype.ContentId` | [Hidden] {security: PluginSecurity} |
| `Class.Decal.RoughnessMapContent` | `Datatype.Content` |  {write: PluginSecurity} |
| `Class.Decal.Shiny` | `float` | [NotReplicated] [Deprecated] |
| `Class.Decal.Specular` | `float` | [NotReplicated] [Deprecated] |
| `Class.Decal.Texture` | `Datatype.ContentId` |  |
| `Class.Decal.TextureContent` | `Datatype.Content` |  |
| `Class.Decal.TexturePack` | `Datatype.ContentId` |  {security: RobloxSecurity} |
| `Class.Decal.Transparency` | `float` |  |
| `Class.Decal.UVOffset` | `Datatype.Vector2` |  |
| `Class.Decal.UVScale` | `Datatype.Vector2` |  |
| `Class.Decal.ZIndex` | `int` |  |

---
title: Texture
type: class
superclass: Decal
---

# Texture

Applies a repeating image texture to the face of a parent `Class.BasePart`.

**Inherits from:** `Class.Decal` > `Class.FaceInstance` > `Class.Instance` > `Class.Object`

## Description

A `Class.Texture` object applies a repeating image texture to the face of a
parent `Class.BasePart`. The affected face is dependent on the
`Class.Texture.Face|Face` property. Unlike `Class.Decal|Decals`, the texture
applied by a `Class.Texture` will repeat when the parent `Class.BasePart` is
resized, with the size of the repeating textures determined by the
`Class.Texture.StudsPerTileU|StudsPerTileU` and
`Class.Texture.StudsPerTileV|StudsPerTileV` properties.

The applied image texture is determined by its
`Class.Texture.ColorMapContent|ColorMapContent` property. For details on how
to upload images, see
[asset management](../../../projects/assets/index.md#asset-management).

For more information, review
[textures and decals](../../../parts/textures-decals.md). See also:

- `Class.Decal` for non-repeating surface images.
- `Class.MeshPart.TextureContent` to apply an image texture to a
  `Class.MeshPart`.
- `Class.SurfaceGui` to apply an `Class.ImageLabel` or `Class.ImageButton` to
  an in-experience 3D object.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Texture.OffsetStudsU` | `float` |  |
| `Class.Texture.OffsetStudsV` | `float` |  |
| `Class.Texture.StudsPerTileU` | `float` |  |
| `Class.Texture.StudsPerTileV` | `float` |  |

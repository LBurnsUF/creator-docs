---
title: WrapTextureTransfer
type: class
superclass: Instance
---

# WrapTextureTransfer

`Class.WrapTextureTransfer` allows a parent `Class.Decal` to be wrapped around
its parent `Class.MeshPart` based on the cage of its `Class.WrapTarget`.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

WrapTextureTransfer provides an alternative projection mode for `Class.Decal`
where this `Class.Decal` is fit to the parent `Class.MeshPart` based on it's
CageMesh provided in `Class.WrapTarget`.

This is useful as it allows fitting of Decals to a wide variety of differently
shaped MeshParts that share a similar WrapTarget CageMesh topology. By
authoring textures that are in the WrapTarget UV space, these textures can be
reused across many different MeshParts with different texture layouts.

- DataModel Structure
  - `Class.MeshPart`
    - `Class.WrapTarget`
    - `Class.Decal`
      - `Class.WrapTextureTransfer`

A way to visualize how this works is to imagine the Decals textures on the
WrapTarget CageMesh, which is wrapped around the MeshPart. These textures are
then projected from the CageMesh onto the MeshPart surface. Geometry that is
internal to the MeshPart, or that is not covered by the CageMesh, will not
receive any projected decal textures. Segmented regions of the target
`Class.MeshPart` are used to improve projection quality near holes or
boundaries in the CageMesh.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.WrapTextureTransfer.ReferenceCageMeshContent` | `Datatype.Content` |  |
| `Class.WrapTextureTransfer.UVMaxBound` | `Datatype.Vector2` |  |
| `Class.WrapTextureTransfer.UVMinBound` | `Datatype.Vector2` |  |

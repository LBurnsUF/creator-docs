---
title: SpecialMesh
type: class
superclass: FileMesh
---

# SpecialMesh

The `Class.SpecialMesh` object applies a mesh to a `Class.BasePart` depending
on the `Class.SpecialMesh.MeshType|MeshType` property.

**Inherits from:** `Class.FileMesh` > `Class.DataModelMesh` > `Class.Instance` > `Class.Object`

## Description

The `Class.SpecialMesh` object applies a mesh to a `Class.BasePart` depending
on the `Class.SpecialMesh.MeshType|MeshType` property. A number of options are
available.

- **Brick** - A block shape, equivalent to a `Class.BlockMesh`
- **Cylinder** - A cylinder, identical to a `Class.Part` with a
  `Class.Part.Shape` of 'Cylinder'
- **FileMesh** - A user uploaded Mesh, equivalent to `Class.FileMesh` that a
  texture can be applied to using the `Class.FileMesh.TextureId` property
- **Head** - A character head shape
- **Sphere** - A sphere shape, similar to a `Class.Part` with a
  `Class.Part.Shape` of 'Ball' but can be freely resized on all axis
- **Wedge** - A wedge shape, identical to a `Class.WedgePart`
- **Torso** - A block with sloped sides, due to be deprecated

Note, each `Class.SpecialMesh.MeshType` will scale differently when using
`Class.DataModelMesh.Scale`, for more information on this please see the page
on `Class.DataModelMesh.Scale`. The SpecialMesh object also exposes the
`Class.DataModelMesh.Offset` property.

It is important to remember that when using a SpecialMesh, only the appearance
of a part changes. The collision model of the part remains the same. For
example, a character will not be able to walk correctly over a mesh as the
mesh geometry is not taken into account.

#### SpecialMesh vs MeshPart

There are currently two ways of using a developer created mesh. They are using
a SpecialMesh with the `Class.SpecialMesh.FileType` set to 'FileMesh', or by
using a `Class.MeshPart`. Although, on the whole, the `Class.MeshPart` object
has superseded the SpecialMesh there are some differences developers should be
aware of.

- `Class.BasePart.Material` displays correctly on the mesh when using a
  `Class.MeshPart` and not when using a SpecialMesh
- `Class.MeshPart|MeshParts` include the `Class.MeshPart.CollisionFidelity`
  property, meaning the collision model of a `Class.MeshPart` can be set to
  resemble the geometry of the mesh. The SpecialMesh object by contrast, uses
  the parent `Class.BasePart|BaseParts` collision model
- The mesh of a `Class.MeshPart` scales on all axis depending on the
  `Class.BasePart.Size|Size` property of the `Class.MeshPart`, the mesh of a
  SpecialMesh does not
- The SpecialMesh object includes the `Class.DataModelMesh.Offset|Offset` and
  `Class.DataModelMesh.Scale|Scale` properties whereas
  `Class.MeshPart|MeshParts` do not
- The `Class.FileMesh.MeshId|MeshId` property of a `Class.SpecialMesh` can be
  changed by a `Class.Script` or `Class.LocalScript` during runtime. The
  `Class.MeshPart.MeshId|MeshId` property of a `Class.MeshPart` can not.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.SpecialMesh.MeshType` | `Enum.MeshType` |  |

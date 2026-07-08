---
title: FileMesh
type: class
superclass: DataModelMesh
---

# FileMesh

The FileMesh object applies a mesh to a `Class.BasePart` when parented to it.
Its properties are inherited by the `Class.SpecialMesh` object.

**Inherits from:** `Class.DataModelMesh` > `Class.Instance` > `Class.Object`

## Description

The FileMesh object applies a textured mesh to a `Class.BasePart` when
parented to it. Its properties are inherited by the `Class.SpecialMesh`
object.

## What is a FileMesh?

FileMeshes allow user uploaded meshes to be applied to a `Class.BasePart`. The
mesh that is applied is dependent on the `Class.FileMesh.MeshId` property. A
texture can also be applied to this mesh using `Class.FileMesh.TextureId`.

Although it is not an abstract class, and can be used by developers, all
`Class.FileMesh` properties are inherited by the `Class.SpecialMesh` object. A
`Class.SpecialMesh` behaves identically to the FileMesh object when its
`Class.SpecialMesh.MeshType` is set to 'FileMesh'. Although both objects are
functional, the `Class.SpecialMesh` object is the official supported class.

For more information on using meshes, please see the `Class.SpecialMesh` page.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.FileMesh.MeshContent` | `Datatype.Content` |  |
| `Class.FileMesh.MeshId` | `Datatype.ContentId` |  |
| `Class.FileMesh.TextureContent` | `Datatype.Content` |  |
| `Class.FileMesh.TextureId` | `Datatype.ContentId` |  |

---
title: WrapDeformer
type: class
superclass: BaseWrap
---

# WrapDeformer

Allows for the real-time deformation of a `Class.MeshPart`.

**Inherits from:** `Class.BaseWrap` > `Class.Instance` > `Class.Object`

## Description

The `Class.WrapDeformer` object provides a low-resolution cage mesh that pairs
with a `Class.WrapTarget` sibling to deform a parent `Class.MeshPart`. The
`Class.MeshPart` geometry is deformed according to the displacement between
pairs of `Class.WrapTarget` cage mesh vertices and `Class.WrapDeformer` cage
mesh vertices. Cage mesh vertices are paired based on UV equivalence.

`Class.WrapDeformer` may be used with avatars or on distinct
`Class.MeshPart|MeshParts`, as long as `Class.WrapTarget` children are present
for the parent `Class.MeshPart|MeshParts`. `Class.WrapDeformer` is similar to
`Class.WrapLayer` but doesn't require layered clothing and can directly deform
`Class.MeshPart|MeshParts` for publishing.

## Methods

### `Class.WrapDeformer:CreateEditableMeshAsync`

``CreateEditableMeshAsync()`` -> `Class.EditableMesh`
  [Yields]

### `Class.WrapDeformer:GetDeformedCFrameAsync`

``GetDeformedCFrameAsync(originalCFrame: `Datatype.CFrame`)`` -> `Datatype.CFrame`
  [Yields]

### `Class.WrapDeformer:SetCageMeshContent`

``SetCageMeshContent(content: `Datatype.Content`, cageOrigin: `Datatype.CoordinateFrame`?)`` -> `null`

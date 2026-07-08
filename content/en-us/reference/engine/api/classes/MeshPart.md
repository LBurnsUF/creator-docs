---
title: MeshPart
type: class
superclass: TriangleMeshPart
---

# MeshPart

A form of `Class.BasePart` that includes a physically simulated custom mesh.

**Inherits from:** `Class.TriangleMeshPart` > `Class.BasePart` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

## Description

`Class.MeshPart` is a form of `Class.BasePart` that includes a physically
simulated custom mesh. Unlike with other mesh classes, such as
`Class.SpecialMesh` and `Class.BlockMesh`, they are not parented to a
`Class.BasePart` but rather behave as a `Class.BasePart` in their own right.

The mesh and texture of a `Class.MeshPart` are determined by the
`Class.MeshPart.MeshId|MeshId` and `Class.MeshPart.TextureID|TextureID`
properties. For more information, see [Meshes](../../../parts/meshes.md).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.MeshPart.DoubleSided` | `bool` |  |
| `Class.MeshPart.HasJointOffset` | `bool` | [Hidden] [Deprecated] {write: NotAccessibleSecurity} |
| `Class.MeshPart.HasSkinnedMesh` | `bool` | [Hidden] {write: NotAccessibleSecurity} |
| `Class.MeshPart.JointOffset` | `Datatype.Vector3` | [Hidden] [Deprecated] {write: NotAccessibleSecurity} |
| `Class.MeshPart.MeshContent` | `Datatype.Content` |  {write: NotAccessibleSecurity} |
| `Class.MeshPart.MeshId` | `Datatype.ContentId` |  {write: NotAccessibleSecurity} |
| `Class.MeshPart.RenderFidelity` | `Enum.RenderFidelity` | [NotReplicated] {write: PluginSecurity} |
| `Class.MeshPart.TextureContent` | `Datatype.Content` |  |
| `Class.MeshPart.TextureID` | `Datatype.ContentId` |  |

## Methods

### `Class.MeshPart:ApplyMesh`

``ApplyMesh(meshPart: `Class.Instance`)`` -> `null`

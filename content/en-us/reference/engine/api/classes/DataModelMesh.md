---
title: DataModelMesh
type: class
superclass: Instance
tags: [NotCreatable, NotBrowsable]
---

# DataModelMesh

The DataModelMesh is an abstract class from which mesh classes descend.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotBrowsable]

## Description

The DataModelMesh is an abstract class from which mesh classes descend.

Mesh classes are objects that, when parented to `Class.BasePart|BaseParts`
alter the appearance of the part to that of a predefined mesh. Note, they only
alter the appearance of the part and not the physics/collision boundaries of
the part. Developers looking to apply a mesh to a part that alters the part's
collision should use `Class.MeshPart|MeshParts`.

Note the `Class.MeshPart` and `Class.CharacterMesh` classes do not descend
from DataModelMesh.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.DataModelMesh.Offset` | `Datatype.Vector3` |  |
| `Class.DataModelMesh.Scale` | `Datatype.Vector3` |  |
| `Class.DataModelMesh.VertexColor` | `Datatype.Vector3` |  |

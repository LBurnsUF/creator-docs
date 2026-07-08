---
title: TriangleMeshPart
type: class
superclass: BasePart
tags: [NotCreatable]
---

# TriangleMeshPart

Abstract intermediate class that manages physical geometry properties for
PartOperations and MeshParts.

**Inherits from:** `Class.BasePart` > `Class.PVInstance` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

TriangleMeshPart is an abstract intermediate class from which `Class.MeshPart`
and `Class.PartOperation` inherit. It was created to consolidate the
management of physical geometry properties between the two sub-classes. It
implements the read-only
`Class.TriangleMeshPart.CollisionFidelity|CollisionFidelity`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.TriangleMeshPart.CollisionFidelity` | `Enum.CollisionFidelity` | [NotReplicated] {write: PluginSecurity} |
| `Class.TriangleMeshPart.FluidFidelity` | `Enum.FluidFidelity` | [NotReplicated] {write: PluginSecurity} |
| `Class.TriangleMeshPart.MeshSize` | `Datatype.Vector3` | [ReadOnly] [NotReplicated] |
| `Class.TriangleMeshPart.UnscaledCofm` | `Datatype.Vector3` | [Hidden] {security: RobloxSecurity} |
| `Class.TriangleMeshPart.UnscaledVolInertiaDiags` | `Datatype.Vector3` | [Hidden] {security: RobloxSecurity} |
| `Class.TriangleMeshPart.UnscaledVolInertiaOffDiags` | `Datatype.Vector3` | [Hidden] {security: RobloxSecurity} |
| `Class.TriangleMeshPart.UnscaledVolume` | `float` | [Hidden] {security: RobloxSecurity} |

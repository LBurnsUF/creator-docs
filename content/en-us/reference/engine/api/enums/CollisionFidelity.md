---
title: CollisionFidelity
type: enum
---

# `Enum.CollisionFidelity`

Determines behavior of the collision hitbox for `Class.MeshPart` and
`Class.PartOperation` instances.

Determines behavior of the collision hitbox for `Class.MeshPart` and
`Class.PartOperation` instances. See
[here](../../../workspace/collisions.md#collision-fidelity) for a visual
representation of the various options.

The `Enum.CollisionFidelity` enum has 5 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.CollisionFidelity.Default` | 0 | Collision model uses a voxel-based convex-hull decomposition that is relatively fast but may not be  |
| `Enum.CollisionFidelity.Hull` | 1 | Collision model uses the convex hull of the visual mesh. |
| `Enum.CollisionFidelity.Box` | 2 | Collision model uses a bounding box that encompasses the visual mesh. |
| `Enum.CollisionFidelity.PreciseConvexDecomposition` | 3 | Collison model uses a convex-hull decomposition of the visual mesh which is computed by a variation  |
| `Enum.CollisionFidelity.Scalable` | 4 |  |

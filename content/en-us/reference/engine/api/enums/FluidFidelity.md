---
title: FluidFidelity
type: enum
---

# `Enum.FluidFidelity`

Determines the geometric representation used to compute aerodynamic forces.

Determines the geometric representation used to compute aerodynamic forces and
torques for `Class.MeshPart` and `Class.PartOperation` instances.

The `Enum.FluidFidelity` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.FluidFidelity.Automatic` | 0 | Let the physics engine select the geometric representation for aerodynamic force and torque calculat |
| `Enum.FluidFidelity.UseCollisionGeometry` | 1 | Use the current collision geometry specified by `Class.TriangleMeshPart.CollisionFidelity` for aerod |
| `Enum.FluidFidelity.UsePreciseGeometry` | 2 | Force the engine to compute aerodynamic forces and torques using a more precise geometry representat |

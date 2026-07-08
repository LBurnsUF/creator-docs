---
title: FluidForces
type: enum
---

# `Enum.FluidForces`

Controls the enablement of aerodynamic forces on parts and assemblies in the
workspace.

Used as an enum value for `Class.Workspace.FluidForces` to control the
enablement of aerodynamic forces on parts and assemblies in the workspace.
Note that this enum is not applicable in scripting and
`Class.Workspace.FluidForces` must be toggled in Studio.

The `Enum.FluidForces` enum has 2 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.FluidForces.Default` | 0 | Aerodynamic forces will not be calculated on any `Class.BasePart/BaseParts`. |
| `Enum.FluidForces.Experimental` | 1 | Aerodynamic forces will be calculated on `Class.BasePart/BaseParts` with `Class.BasePart.EnableFluid |

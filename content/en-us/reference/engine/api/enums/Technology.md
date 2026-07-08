---
title: Technology
type: enum
---

# `Enum.Technology`

Enum used by `Class.Lighting.Technology` to represent the different lighting
systems available for rendering the 3D world.

This enum represents the different lighting systems available for rendering
the 3D world. It is used by the `Class.Lighting.Technology` property.

Note that `Class.Lighting.Technology` has been superseded by
`Class.Lighting.LightingStyle|LightingStyle` which determines the artistic
intent behind lighting, and
`Class.Lighting.PrioritizeLightingQuality|PrioritizeLightingQuality` which
indicates whether you prefer lighting/shading quality or view distance to
scale down first.

The `Enum.Technology` enum has 6 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.Technology.Legacy` | 0 |  |
| `Enum.Technology.Voxel` | 1 | Uses a 4&times;4&times;4 voxel map for light and shadow calculation. |
| `Enum.Technology.Compatibility` | 2 | Simulates the removed legacy technology and is now deprecated. To achieve a similar look, use `Voxel |
| `Enum.Technology.ShadowMap` | 3 | Features shadow mapping that produces more realistic and crisp shadows from sunlight or directional  |
| `Enum.Technology.Future` | 4 | Features the most advanced technology for high-fidelity lighting and shadows. |
| `Enum.Technology.Unified` | 5 |  |

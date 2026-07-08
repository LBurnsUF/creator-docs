---
title: AlphaMode
type: enum
---

# `Enum.AlphaMode`

Used by `Class.SurfaceAppearance.AlphaMode` to determine how the alpha channel
of the `Class.SurfaceAppearance.ColorMap` of a `Class.SurfaceAppearance` is
used.

Used by `Class.SurfaceAppearance.AlphaMode` to determine how the alpha channel
of the `Class.SurfaceAppearance.ColorMap` of a `Class.SurfaceAppearance` is
used.

The `Enum.AlphaMode` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.AlphaMode.Overlay` | 0 | Overlays the `Class.SurfaceAppearance.ColorMap/ColorMap` on top of the underlying part color based o |
| `Enum.AlphaMode.Transparency` | 1 | Uses the `Class.SurfaceAppearance.ColorMap/ColorMap` alpha channel to control the transparency of th |
| `Enum.AlphaMode.TintMask` | 2 | Uses the `Class.SurfaceAppearance.ColorMap/ColorMap` alpha channel to control the amount of `Class.S |
| `Enum.AlphaMode.Opaque` | 3 | Ignores the `Class.SurfaceAppearance.ColorMap/ColorMap` alpha channel and assumes an opacity value o |

---
title: VolumetricAudio
type: enum
---

# `Enum.VolumetricAudio`

Controls how the engine renders volumetric audio effects.

Controls how the engine renders volumetric audio effects, allowing sound to
emanate from the surface of a `Class.Part` rather than a single point in
space.

The `Enum.VolumetricAudio` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.VolumetricAudio.Disabled` | 0 | Volumetric audio is disabled; sound emanates from a single point. |
| `Enum.VolumetricAudio.Automatic` | 1 | Currently equivalent to `Enum.VolumetricAudio.Disabled`. |
| `Enum.VolumetricAudio.Enabled` | 2 | Volumetric audio is enabled; sound emanates from the object's volume. |

---
title: SurfaceAppearance
type: class
superclass: Instance
---

# SurfaceAppearance

An object that allows developers to override the appearance of a MeshPart with
advanced graphics options.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

**SurfaceAppearance** objects let you override the appearance of a
`Class.MeshPart` with advanced graphics options. Most notably, it can apply a
set of **Physically‑Based Rendering** (PBR) texture images, or maps, on a
single object. Combining multiple texture maps can more accurately simulate
color, roughness, and reflectivity in any lighting environment and can enhance
the visual elements of your assets and environment; see
[PBR Textures](../../../art/modeling/surface-appearance.md) for more details.

<figure>
<img src="/assets/modeling/surface-appearance/SurfaceAppearance-Example-1.jpg" width="405" alt="A realistic leafy bush" />
<img src="/assets/modeling/surface-appearance/SurfaceAppearance-Example-3.jpg" width="405" alt="A realistic mossy rock" />
</figure>

Appearance of this object on a `Class.MeshPart` depends on the user's device
and graphics quality level. For best results, you may want to preview your
content with different quality level settings.

Note that most `Class.SurfaceAppearance` properties cannot be modified by
scripts, as the necessary pre-processing is usually too expensive during
runtime.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.SurfaceAppearance.AlphaMode` | `Enum.AlphaMode` |  |
| `Class.SurfaceAppearance.Color` | `Datatype.Color3` |  |
| `Class.SurfaceAppearance.ColorMap` | `Datatype.ContentId` |  {security: PluginSecurity} |
| `Class.SurfaceAppearance.ColorMapContent` | `Datatype.Content` | [Hidden] {write: PluginSecurity} |
| `Class.SurfaceAppearance.EmissiveMaskContent` | `Datatype.Content` |  {write: PluginSecurity} |
| `Class.SurfaceAppearance.EmissiveStrength` | `float` |  |
| `Class.SurfaceAppearance.EmissiveTint` | `Datatype.Color3` |  |
| `Class.SurfaceAppearance.MetalnessMap` | `Datatype.ContentId` |  {security: PluginSecurity} |
| `Class.SurfaceAppearance.MetalnessMapContent` | `Datatype.Content` | [Hidden] {write: PluginSecurity} |
| `Class.SurfaceAppearance.NormalMap` | `Datatype.ContentId` |  {security: PluginSecurity} |
| `Class.SurfaceAppearance.NormalMapContent` | `Datatype.Content` | [Hidden] {write: PluginSecurity} |
| `Class.SurfaceAppearance.ResampleMode` | `Enum.ResamplerMode` |  |
| `Class.SurfaceAppearance.RoughnessMap` | `Datatype.ContentId` |  {security: PluginSecurity} |
| `Class.SurfaceAppearance.RoughnessMapContent` | `Datatype.Content` | [Hidden] {write: PluginSecurity} |
| `Class.SurfaceAppearance.TexturePack` | `Datatype.ContentId` |  {read: RobloxScriptSecurity, write: RobloxSecurity} |

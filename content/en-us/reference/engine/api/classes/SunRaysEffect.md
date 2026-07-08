---
title: SunRaysEffect
type: class
superclass: PostEffect
---

# SunRaysEffect

Renders dynamic rays from the sun.

**Inherits from:** `Class.PostEffect` > `Class.Instance` > `Class.Object`

## Description

The **SunRaysEffect** renders a halo of light around sun. The halo is
shaped/blocked by world objects between the `Class.Workspace.CurrentCamera`
and the sun.

Like other post-processing effects, **SunRaysEffect** will only work while
`Class.PostEffect.Enabled|Enabled` and when parented to `Class.Lighting` or
`Class.Workspace.CurrentCamera`. Also, it may not render on low-end devices,
and it may render differently depending on your Studio settings (see the
**Quality Level** settings in **Rendering** &rarr; **Performance**).

For more details on this effect and others, see
[Post-Processing Effects](../../../environment/post-processing-effects.md).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.SunRaysEffect.Intensity` | `float` |  |
| `Class.SunRaysEffect.Spread` | `float` |  |

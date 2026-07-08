---
title: BloomEffect
type: class
superclass: PostEffect
---

# BloomEffect

Simulates the camera viewing a very bright light.

**Inherits from:** `Class.PostEffect` > `Class.Instance` > `Class.Object`

## Description

The **BloomEffect** simulates the camera viewing a very bright light. It
causes brighter colors to glow, similar to applying the neon
`Class.BasePart.Material|Material` to everything, including the `Class.Sky`.
Multiple **BloomEffect** objects can be applied at once and they will compose
their effects together.

Like other post-processing effects, **BloomEffect** will only work while
`Class.PostEffect.Enabled|Enabled` and when parented to `Class.Lighting` or
`Class.Workspace.CurrentCamera`. Also, it may render differently depending on
your Studio settings (see the **Quality Level** settings in **Rendering**
&rarr; **Performance**).

For more details on this effect and others, see
[Post-Processing Effects](../../../environment/post-processing-effects.md).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.BloomEffect.Intensity` | `float` |  |
| `Class.BloomEffect.Size` | `float` |  |
| `Class.BloomEffect.Threshold` | `float` |  |

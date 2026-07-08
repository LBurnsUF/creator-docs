---
title: BlurEffect
type: class
superclass: PostEffect
---

# BlurEffect

Applies a blur to the entire game world.

**Inherits from:** `Class.PostEffect` > `Class.Instance` > `Class.Object`

## Description

The **BlurEffect** applies a Gaussian blur to the entire rendered game world.
The strength of the blur is controlled by the `Class.BlurEffect.Size`. Only
one **BlurEffect** can be applied at once (the instance with the greatest
`Class.BlurEffect.Size|Size` takes priority).

Like other post-processing effects, **BlurEffect** will only work while
`Class.PostEffect.Enabled|Enabled` and when parented to `Class.Lighting` or
`Class.Workspace.CurrentCamera`. Also, it may render differently on low-end
devices and/or depending on your Studio settings (see the **Quality Level**
settings in **Rendering** &rarr; **Performance**).

For more details on this effect and others, see
[Post-Processing Effects](../../../environment/post-processing-effects.md).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.BlurEffect.Size` | `float` |  |

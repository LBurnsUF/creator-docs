---
title: DepthOfFieldEffect
type: class
superclass: PostEffect
---

# DepthOfFieldEffect

Simulates a camera lens by blurring parts of a scene not in focus.

**Inherits from:** `Class.PostEffect` > `Class.Instance` > `Class.Object`

## Description

The **DepthOfFieldEffect** simulates a camera lens by blurring parts of a
scene not in focus. Distant objects can be blurred or this effect can be used
to focus on specific parts of a scene, like an item in an in-game shop.

Like other post-processing effects, **DepthOfFieldEffect** will only work
while `Class.PostEffect.Enabled|Enabled` and when parented to `Class.Lighting`
or `Class.Workspace.CurrentCamera`. Also, it may render differently on low-end
devices or depending on your Studio settings (see the **Quality Level**
settings in **Rendering** &rarr; **Performance**).

For more details on this effect and others, see
[Post-Processing Effects](../../../environment/post-processing-effects.md).

<img src="../../../assets/engine-api/classes/DepthOfFieldEffect/Depth-Of-Field-Diagram.svg" />

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.DepthOfFieldEffect.FarIntensity` | `float` |  |
| `Class.DepthOfFieldEffect.FocusDistance` | `float` |  |
| `Class.DepthOfFieldEffect.InFocusRadius` | `float` |  |
| `Class.DepthOfFieldEffect.NearIntensity` | `float` |  |

---
title: ColorCorrectionEffect
type: class
superclass: PostEffect
---

# ColorCorrectionEffect

Adjusts color-related properties of the rendered world like saturation, tint,
brightness, and contrast.

**Inherits from:** `Class.PostEffect` > `Class.Instance` > `Class.Object`

## Description

`Class.ColorCorrectionEffect` can be used to adjust several color-related
properties at once, including
`Class.ColorCorrectionEffect.Saturation|Saturation`,
`Class.ColorCorrectionEffect.TintColor|TintColor`,
`Class.ColorCorrectionEffect.Brightness|Brightness` and
`Class.ColorCorrectionEffect.Contrast|Contrast`. It's useful for fine-tuning
the visual aesthetic of a world or communicating status effects to the player.
Multiple `Class.ColorCorrectionEffect` objects can be applied at the same time
and they will compose their effects together.

Like other
[post-processing effects](../../../environment/post-processing-effects.md),
`Class.ColorCorrectionEffect` will only work while
`Class.PostEffect.Enabled|Enabled` and when parented to `Class.Lighting` or
`Class.Workspace.CurrentCamera`. Also, it may render differently depending on
your Studio settings (see **Editor&nbsp;Quality&nbsp;Level** in
**Rendering**).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ColorCorrectionEffect.Brightness` | `float` |  |
| `Class.ColorCorrectionEffect.Contrast` | `float` |  |
| `Class.ColorCorrectionEffect.Saturation` | `float` |  |
| `Class.ColorCorrectionEffect.TintColor` | `Datatype.Color3` |  |

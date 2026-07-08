---
title: ColorGradingEffect
type: class
superclass: PostEffect
---

# ColorGradingEffect

Modifies how color values calculated by the renderer should be converted to
the screen's color range.

**Inherits from:** `Class.PostEffect` > `Class.Instance` > `Class.Object`

## Description

The **ColorGradingEffect** effect modifies how color values calculated by the
renderer should be converted to the screen's color range, impacting the mood
and appearance of your place.

**ColorGradingEffect** is expected to be parented to `Class.Lighting` and will
be ignored if parented elsewhere. Multiple instances cannot be combined and
only the most recently parented instance to `Class.Lighting` will be applied.

For more details on this effect and others, see
[Post-Processing Effects](../../../environment/post-processing-effects.md).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ColorGradingEffect.TonemapperPreset` | `Enum.TonemapperPreset` |  |

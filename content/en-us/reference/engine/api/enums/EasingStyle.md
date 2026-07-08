---
title: EasingStyle
type: enum
---

# `Enum.EasingStyle`

Enum used with `Datatype.TweenInfo|TweenInfo.new` to control the motion of a
`Class.Tween`.

These enum values are passed to `Datatype.TweenInfo|TweenInfo.new()` to
control the motion of a `Class.Tween`. The following graphs reflect easing
styles for `Enum.EasingDirection|Enum.EasingDirection.In`. For graphs
reflecting `Enum.EasingDirection|Enum.EasingDirection.Out` and
`Enum.EasingDirection|Enum.EasingDirection.InOut`, see
[UI&nbsp;Animations](../../../ui/animation.md#style).

<img src="/assets/engine-api/enums/EasingStyle/Easing-Styles-In.png" width="800" alt="Graphs of EasingStyle variations with an 'In' EasingDirection." />

The `Enum.EasingStyle` enum has 11 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.EasingStyle.Linear` | 0 | Moves at a constant speed. |
| `Enum.EasingStyle.Sine` | 1 | Speed is determined by a sine wave for a gentle easing motion. |
| `Enum.EasingStyle.Back` | 2 | Slightly overshoots the target, then backs into place. |
| `Enum.EasingStyle.Quad` | 3 | Similar to `Sine` but with a slightly sharper curve based on quadratic interpolation. |
| `Enum.EasingStyle.Quart` | 4 | Similar to `Cubic` but with an even sharper curve based on quartic interpolation. |
| `Enum.EasingStyle.Quint` | 5 | Similar to `Quart` but with an even sharper curve based on quintic interpolation. |
| `Enum.EasingStyle.Bounce` | 6 | Bounces backwards multiple times after reaching the target, before eventually settling. |
| `Enum.EasingStyle.Elastic` | 7 | Moves as if attached to a rubber band, overshooting the target several times. |
| `Enum.EasingStyle.Exponential` | 8 | The sharpest curve based on exponential interpolation. |
| `Enum.EasingStyle.Circular` | 9 | Follows a circular arc, such that acceleration is more sudden and deceleration more gradual versus ` |
| `Enum.EasingStyle.Cubic` | 10 | Similar to `Quad` but with a slightly sharper curve based on cubic interpolation. |

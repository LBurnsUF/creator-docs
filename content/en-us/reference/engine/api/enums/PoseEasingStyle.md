---
title: PoseEasingStyle
type: enum
---

# `Enum.PoseEasingStyle`

The `Enum.PoseEasingStyle` enum has 6 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.PoseEasingStyle.Linear` | 0 | Poses interpolate linearly between key frames. |
| `Enum.PoseEasingStyle.Constant` | 1 | Poses do not interpolate but snap to the key frame indicated by the `Enum.PoseEasingDirection`. |
| `Enum.PoseEasingStyle.Elastic` | 2 | Pose interpolation will overshoot like it is elastic. |
| `Enum.PoseEasingStyle.Cubic` | 3 | Deprecated - Use `Enum.PoseEasingStyle.CubicV2`. Pose interpolation is a cubic curve between keyfram |
| `Enum.PoseEasingStyle.Bounce` | 4 | Pose interpolation produces a bounce like effect between key frames. |
| `Enum.PoseEasingStyle.CubicV2` | 5 | Pose interpolation is a cubic curve between keyframes based on `Enum.PoseEasingDirection`. |

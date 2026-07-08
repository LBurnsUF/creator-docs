---
title: PoseEasingDirection
type: enum
---

# `Enum.PoseEasingDirection`

Used exclusively by Pose.EasingDirection to specify direction of the
EasingStyle curve.

When a Pose has an EasingStyle which is not symmetric, the EasingDirection
determines if the curve is applied from previous keyframe to next, next
keyframe to previous, or in both directions by using two copies of the curve
back to back. For the symmetric Linear and Constant EasingStyles, this
property has no effect. For legacy compatibility reasons, the use of In and
Out are backwards from how these terms are used by most other animation tools
and by TweenService.

The `Enum.PoseEasingDirection` enum has 3 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.PoseEasingDirection.In` | 0 | The EasingStyle curve is reversed, with the easing becoming linear as it approaches the next keyfram |
| `Enum.PoseEasingDirection.Out` | 1 | EasingStyle curves are applied in the forward direction, from the current keyframe to the next. |
| `Enum.PoseEasingDirection.InOut` | 2 | Two easing curves are applied back-to-back with the linear ends of the curves meeting in the middle. |

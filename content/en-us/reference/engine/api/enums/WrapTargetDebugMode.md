---
title: WrapTargetDebugMode
type: enum
---

# `Enum.WrapTargetDebugMode`

The Studio-only property for quickly visualizing and debugging meshes with
only outer cages.

The Studio-only property for quickly visualizing and debugging meshes with
only outer cages.

This debug visualization only works when the WrapTarget is active and does not
work if WrapTarget is not active or incorrectly configured.

The `Enum.WrapTargetDebugMode` enum has 10 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.WrapTargetDebugMode.None` | 0 | This debug rendering mode does nothing, and this is the default value. |
| `Enum.WrapTargetDebugMode.TargetCageOriginal` | 1 | This debug mode shows the original cage mesh as it was created. |
| `Enum.WrapTargetDebugMode.TargetCageCompressed` | 2 | This debug mode shows corresponding cage mesh compressed by clothing layers above it. This debug mod |
| `Enum.WrapTargetDebugMode.TargetCageInterface` | 3 | This debug mode shows the resulting cage mesh for the corresponding Wrap Instance. This debug mode i |
| `Enum.WrapTargetDebugMode.TargetLayerCageOriginal` | 4 | The same as TargetCageOriginal but affects all WrapTargets that belong to the Wrap Deformer simultan |
| `Enum.WrapTargetDebugMode.TargetLayerCageCompressed` | 5 | The same as TargetCageCompressed but affects all WrapTargets that belong to the Wrap Deformer simult |
| `Enum.WrapTargetDebugMode.TargetLayerInterface` | 6 | The same as TargetCageInterface but affects all WrapTargets that belong to the Wrap Deformer simulta |
| `Enum.WrapTargetDebugMode.Rbf` | 7 | This debug mode visualizes the internal RBF solver state. You can estimate the wrap deformer expecte |
| `Enum.WrapTargetDebugMode.OuterCageDetail` | 8 |  |
| `Enum.WrapTargetDebugMode.PreWrapDeformerCage` | 9 |  |

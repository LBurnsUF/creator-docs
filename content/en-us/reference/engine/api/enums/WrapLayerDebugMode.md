---
title: WrapLayerDebugMode
type: enum
---

# `Enum.WrapLayerDebugMode`

The Studio-only property for quickly visualizing and debugging meshes with
inner cage and outer cages.

The Studio-only property for quickly visualizing and debugging meshes with
inner and outer cages.

This debug visualization only works when the WrapLayer is active and does not
work if WrapLayer is not active or incorrectly configured.

The `Enum.WrapLayerDebugMode` enum has 16 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.WrapLayerDebugMode.None` | 0 | This debug rendering mode does nothing. This is the default value. |
| `Enum.WrapLayerDebugMode.BoundCage` | 1 | This debug mode visualizes corresponding cage mesh vertices bound to an underlying `Class.WrapTarget |
| `Enum.WrapLayerDebugMode.LayerCage` | 2 | This debug mode shows the resulting layer mesh as a whole. The deformer will use vertex locations fr |
| `Enum.WrapLayerDebugMode.BoundCageAndLinks` | 3 | The same as BoundCage but also visualizes how bound vertices were moved. You can use this mode to id |
| `Enum.WrapLayerDebugMode.Reference` | 4 | This debug mode shows the original inner cage mesh as it was created. |
| `Enum.WrapLayerDebugMode.Rbf` | 5 | This debug mode visualizes the internal RBF solver state. You can estimate the wrap deformer's expec |
| `Enum.WrapLayerDebugMode.OuterCage` | 6 | This debug mode shows the original outer cage mesh as it was created. |
| `Enum.WrapLayerDebugMode.ReferenceMeshAfterMorph` | 7 |  |
| `Enum.WrapLayerDebugMode.HSROuterDetail` | 8 |  |
| `Enum.WrapLayerDebugMode.HSROuter` | 9 |  |
| `Enum.WrapLayerDebugMode.HSRInner` | 10 |  |
| `Enum.WrapLayerDebugMode.HSRInnerReverse` | 11 |  |
| `Enum.WrapLayerDebugMode.LayerCageFittedToBase` | 12 |  |
| `Enum.WrapLayerDebugMode.LayerCageFittedToPrev` | 13 |  |
| `Enum.WrapLayerDebugMode.PreWrapDeformerOuterCage` | 14 |  |
| `Enum.WrapLayerDebugMode.SkinningTransfer` | 15 |  |

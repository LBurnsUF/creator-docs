---
title: ModelLevelOfDetail
type: enum
---

# `Enum.ModelLevelOfDetail`

Controls the level of detail for `Class.Model|Models` in experiences with
instance streaming enabled.

Controls the level of detail for `Class.Model|Models` in experiences with
instance [streaming](../../../workspace/streaming/index.md) enabled. Composite
or imposter meshes do not support physics, collision detection, or raycasting.

<table>
<tbody>
<tr>
<td>
<figure>
<img src="/assets/modeling/model-objects/LevelOfDetail-Original.jpg" width="270" />
<figcaption>Original model</figcaption>
</figure>
</td>
<td>
<figure>
<img src="/assets/modeling/model-objects/LevelOfDetail-Slim.jpg" width="270" />
<figcaption>Lightweight SLIM mesh</figcaption>
</figure>
</td>
<td>
<figure>
<img src="/assets/modeling/model-objects/LevelOfDetail-Imposter.jpg" width="270" />
<figcaption>Low-res "imposter" mesh</figcaption>
</figure>
</td>
</tr>
</tbody>
</table>

The `Enum.ModelLevelOfDetail` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.ModelLevelOfDetail.Automatic` | 0 | Default behavior, currently equivalent to `Disabled`. |
| `Enum.ModelLevelOfDetail.StreamingMesh` | 1 | A lower resolution "imposter" mesh (colored, coarse mesh that wraps around all child parts of the mo |
| `Enum.ModelLevelOfDetail.Disabled` | 2 | A lower resolution mesh will not be displayed. |
| `Enum.ModelLevelOfDetail.SLIM` | 4 | A **SLIM** model (Scalable Lightweight Interactive Model) renders a composite of all child parts at  |

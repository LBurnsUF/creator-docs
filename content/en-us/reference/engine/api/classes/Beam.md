---
title: Beam
type: class
superclass: Instance
---

# Beam

Connects two `Class.Attachment|Attachments` by drawing a texture between them.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

A **Beam** object connects two `Class.Attachment|Attachments` by drawing a
texture between them.

To display, a beam must be a descendant of the `Class.Workspace` with its
`Class.Beam.Attachment0|Attachment0` and `Class.Beam.Attachment1|Attachment1`
properties set to `Class.Attachment|Attachments` also descending from the
`Class.Workspace`.

The beam's appearance can be customized using the range of properties outlined
below. Also see the [Beams](../../../effects/beams.md) guide for visual
examples.

#### Beam Curvature

Beams are configured to use a cubic Bézier curve formed by four control
points. This means they are not constrained to straight lines and the curve of
the beam can be modified by changing `Class.Beam.CurveSize0|CurveSize0`,
`Class.Beam.CurveSize1|CurveSize1`, and the orientation of the beam's
`Class.Attachment|Attachments`.

- **P0** — The start of the beam; position of
  `Class.Beam.Attachment0|Attachment0`.
- **P1** — `Class.Beam.CurveSize0|CurveSize0` studs away from
  `Class.Beam.Attachment0|Attachment0`, in the positive **X** direction of
  `Class.Beam.Attachment0|Attachment0`.
- **P2** — `Class.Beam.CurveSize1|CurveSize1` studs away from
  `Class.Beam.Attachment1|Attachment1`, in the negative **X** direction of
  `Class.Beam.Attachment1|Attachment1`.
- **P3** — The end of the beam; position of
  `Class.Beam.Attachment1|Attachment1`

<img src="/assets/engine-api/classes/Beam/Curvature-Diagram.png" width="800" alt="Beam curvature diagram" />

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Beam.Attachment0` | `Class.Attachment` |  |
| `Class.Beam.Attachment1` | `Class.Attachment` |  |
| `Class.Beam.Brightness` | `float` |  |
| `Class.Beam.Color` | `Datatype.ColorSequence` |  |
| `Class.Beam.CurveSize0` | `float` |  |
| `Class.Beam.CurveSize1` | `float` |  |
| `Class.Beam.Enabled` | `bool` |  |
| `Class.Beam.FaceCamera` | `bool` |  |
| `Class.Beam.LightEmission` | `float` |  |
| `Class.Beam.LightInfluence` | `float` |  |
| `Class.Beam.LocalTransparencyModifier` | `float` | [Hidden] [NotReplicated] |
| `Class.Beam.Segments` | `int` |  |
| `Class.Beam.Texture` | `Datatype.ContentId` |  |
| `Class.Beam.TextureContent` | `Datatype.Content` |  |
| `Class.Beam.TextureLength` | `float` |  |
| `Class.Beam.TextureMode` | `Enum.TextureMode` |  |
| `Class.Beam.TextureSpeed` | `float` |  |
| `Class.Beam.Transparency` | `Datatype.NumberSequence` |  |
| `Class.Beam.Width0` | `float` |  |
| `Class.Beam.Width1` | `float` |  |
| `Class.Beam.ZOffset` | `float` |  |

## Methods

### `Class.Beam:SetTextureOffset`

``SetTextureOffset(offset: `float`)`` -> `null`

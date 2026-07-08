---
title: Attachment
type: class
superclass: Instance
---

# Attachment

Defines a point and orientation relative to an ancestor `Class.PVInstance`,
`Class.Bone`, or another `Class.Attachment`.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

An `Attachment` defines a point and orientation relative to an ancestor
`Class.PVInstance`, `Class.Bone`, or another `Attachment`. The offset is
stored in the `Class.Attachment.CFrame|CFrame` property. The offset can also
be set through other properties, such as
`Class.Attachment.WorldCFrame|WorldCFrame`.

If no ancestral `Class.PVInstance` or `Class.Attachment` exists, then
`Class.Attachment.CFrame|CFrame` and
`Class.Attachment.WorldCFrame|WorldCFrame` are the same.

Attachments are used by several kinds of `Class.Constraint|Constraints` and
are also valid alternatives to `Class.BasePart` as a parent for objects such
as:

- `Class.ParticleEmitter|ParticleEmitters` which will emit particles from the
  attachment's specific position/orientation instead of the `Class.BasePart`
  bounds.

- Light-emitting objects like `Class.PointLight` and `Class.SpotLight` which
  will shine from the attachment's position/orientation instead of the
  `Class.BasePart` center.

- `Class.AudioEmitter` which will use the attachment's position as the audio's
  point of emission.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Attachment.Axis` | `Datatype.Vector3` | [NotReplicated] |
| `Class.Attachment.CFrame` | `Datatype.CFrame` |  |
| `Class.Attachment.Orientation` | `Datatype.Vector3` | [Hidden] [NotReplicated] |
| `Class.Attachment.Position` | `Datatype.Vector3` | [Hidden] [NotReplicated] |
| `Class.Attachment.Rotation` | `Datatype.Vector3` | [Hidden] [NotReplicated] [Deprecated] |
| `Class.Attachment.SecondaryAxis` | `Datatype.Vector3` | [NotReplicated] |
| `Class.Attachment.Visible` | `bool` |  |
| `Class.Attachment.WorldAxis` | `Datatype.Vector3` | [NotReplicated] |
| `Class.Attachment.WorldCFrame` | `Datatype.CFrame` | [NotReplicated] |
| `Class.Attachment.WorldOrientation` | `Datatype.Vector3` | [Hidden] [NotReplicated] |
| `Class.Attachment.WorldPosition` | `Datatype.Vector3` | [Hidden] [NotReplicated] |
| `Class.Attachment.WorldRotation` | `Datatype.Vector3` | [Hidden] [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.Attachment.WorldSecondaryAxis` | `Datatype.Vector3` | [NotReplicated] |

## Methods

### `Class.Attachment:GetAxis`

``GetAxis()`` -> `Datatype.Vector3`
  [Deprecated]

### `Class.Attachment:GetConstraints`

``GetConstraints()`` -> `Datatype.Instances`

### `Class.Attachment:GetSecondaryAxis`

``GetSecondaryAxis()`` -> `Datatype.Vector3`
  [Deprecated]

### `Class.Attachment:SetAxis`

``SetAxis(axis: `Datatype.Vector3`)`` -> `null`
  [Deprecated]

### `Class.Attachment:SetSecondaryAxis`

``SetSecondaryAxis(axis: `Datatype.Vector3`)`` -> `null`
  [Deprecated]

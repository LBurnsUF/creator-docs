---
title: ParticleEmitter
type: class
superclass: Instance
---

# ParticleEmitter

A special object that emits customizable 2D particles into the world.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

A **ParticleEmitter** is a special object that emits customizable 2D particles
into the world. To emit and render particles, it must be parented to a
`Class.BasePart` or an `Class.Attachment` within such a part. When parented to
a `Class.BasePart`, particles spawn randomly within the part's bounding box or
[shape](../../../effects/particle-emitters.md#shape); when parented to an
`Class.Attachment`, particles spawn from the attachment's position.

Particles emit automatically when the emitter is
`Class.ParticleEmitter.Enabled|Enabled` with a non-zero
`Class.ParticleEmitter.Rate|Rate`, or manually when the
`Class.ParticleEmitter:Emit()|Emit` method is called. With a non-zero
`Class.ParticleEmitter.Speed|Speed`, particles are set in motion outwards
and/or inwards, depending on the `Class.ParticleEmitter.ShapeInOut|ShapeInOut`
property.

By default, particles face the camera, but the
`Class.ParticleEmitter.Orientation|Orientation` can be modified to respect the
particle velocity instead.

During the `Class.ParticleEmitter.Lifetime|Lifetime` of the particles, they
can change appearance according to the `Class.ParticleEmitter.Color|Color` and
`Class.ParticleEmitter.Size|Size`. Their motion can change over time according
to the `Class.ParticleEmitter.Drag|Drag` and
`Class.ParticleEmitter.Acceleration|Acceleration` properties, and they can
also move as their parent moves when they are
`Class.ParticleEmitter.LockedToPart|LockedToPart` or have a non-zero
`Class.ParticleEmitter.VelocityInheritance|VelocityInheritance`.

To learn more about creating and customizing particle emitters, see
[Particle Emitters](../../../effects/particle-emitters.md).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ParticleEmitter.Acceleration` | `Datatype.Vector3` |  |
| `Class.ParticleEmitter.Brightness` | `float` |  |
| `Class.ParticleEmitter.Color` | `Datatype.ColorSequence` |  |
| `Class.ParticleEmitter.Drag` | `float` |  |
| `Class.ParticleEmitter.EmissionDirection` | `Enum.NormalId` |  |
| `Class.ParticleEmitter.Enabled` | `bool` |  |
| `Class.ParticleEmitter.FlipbookBlendFrames` | `bool` |  |
| `Class.ParticleEmitter.FlipbookFramerate` | `Datatype.NumberRange` |  |
| `Class.ParticleEmitter.FlipbookIncompatible` | `string` |  |
| `Class.ParticleEmitter.FlipbookLayout` | `Enum.ParticleFlipbookLayout` |  |
| `Class.ParticleEmitter.FlipbookMode` | `Enum.ParticleFlipbookMode` |  |
| `Class.ParticleEmitter.FlipbookSizeX` | `int` |  |
| `Class.ParticleEmitter.FlipbookSizeY` | `int` |  |
| `Class.ParticleEmitter.FlipbookStartRandom` | `bool` |  |
| `Class.ParticleEmitter.Lifetime` | `Datatype.NumberRange` |  |
| `Class.ParticleEmitter.LightEmission` | `float` |  |
| `Class.ParticleEmitter.LightInfluence` | `float` |  |
| `Class.ParticleEmitter.LocalTransparencyModifier` | `float` | [Hidden] [NotReplicated] |
| `Class.ParticleEmitter.LockedToPart` | `bool` |  |
| `Class.ParticleEmitter.Orientation` | `Enum.ParticleOrientation` |  |
| `Class.ParticleEmitter.Rate` | `float` |  |
| `Class.ParticleEmitter.RotSpeed` | `Datatype.NumberRange` |  |
| `Class.ParticleEmitter.Rotation` | `Datatype.NumberRange` |  |
| `Class.ParticleEmitter.Shape` | `Enum.ParticleEmitterShape` |  |
| `Class.ParticleEmitter.ShapeInOut` | `Enum.ParticleEmitterShapeInOut` |  |
| `Class.ParticleEmitter.ShapePartial` | `float` |  |
| `Class.ParticleEmitter.ShapeStyle` | `Enum.ParticleEmitterShapeStyle` |  |
| `Class.ParticleEmitter.Size` | `Datatype.NumberSequence` |  |
| `Class.ParticleEmitter.Speed` | `Datatype.NumberRange` |  |
| `Class.ParticleEmitter.SpreadAngle` | `Datatype.Vector2` |  |
| `Class.ParticleEmitter.Squash` | `Datatype.NumberSequence` |  |
| `Class.ParticleEmitter.Texture` | `Datatype.ContentId` |  |
| `Class.ParticleEmitter.TextureContent` | `Datatype.Content` |  |
| `Class.ParticleEmitter.TimeScale` | `float` |  |
| `Class.ParticleEmitter.Transparency` | `Datatype.NumberSequence` |  |
| `Class.ParticleEmitter.VelocityInheritance` | `float` |  |
| `Class.ParticleEmitter.VelocitySpread` | `float` | [NotReplicated] [Deprecated] |
| `Class.ParticleEmitter.WindAffectsDrag` | `bool` |  |
| `Class.ParticleEmitter.ZOffset` | `float` |  |

## Methods

### `Class.ParticleEmitter:Clear`

``Clear()`` -> `null`

### `Class.ParticleEmitter:Emit`

``Emit(particleCount: `int`)`` -> `null`

### `Class.ParticleEmitter:FastForward`

``FastForward(numFrames: `int`)`` -> `null`
   {security: RobloxScriptSecurity}

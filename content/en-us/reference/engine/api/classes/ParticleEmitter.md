---
title: ParticleEmitter
type: class
superclass: Instance
---

# ParticleEmitter

**Inherits**: Instance > Object

## Properties

- **Acceleration**: `Vector3`
- **Brightness**: `float`
- **Color**: `ColorSequence`
- **Drag**: `float`
- **EmissionDirection**: `NormalId`
- **Enabled**: `bool`
- **FlipbookBlendFrames**: `bool`
- **FlipbookFramerate**: `NumberRange`
- **FlipbookIncompatible**: `string`
- **FlipbookLayout**: `ParticleFlipbookLayout`
- **FlipbookMode**: `ParticleFlipbookMode`
- **FlipbookSizeX**: `int`
- **FlipbookSizeY**: `int`
- **FlipbookStartRandom**: `bool`
- **Lifetime**: `NumberRange`
- **LightEmission**: `float`
- **LightInfluence**: `float`
- **LocalTransparencyModifier**: `float` [Hidden] [NotReplicated]
- **LockedToPart**: `bool`
- **Orientation**: `ParticleOrientation`
- **Rate**: `float`
- **RotSpeed**: `NumberRange`
- **Rotation**: `NumberRange`
- **Shape**: `ParticleEmitterShape`
- **ShapeInOut**: `ParticleEmitterShapeInOut`
- **ShapePartial**: `float`
- **ShapeStyle**: `ParticleEmitterShapeStyle`
- **Size**: `NumberSequence`
- **Speed**: `NumberRange`
- **SpreadAngle**: `Vector2`
- **Squash**: `NumberSequence`
- **Texture**: `ContentId`
- **TextureContent**: `Content`
- **TimeScale**: `float`
- **Transparency**: `NumberSequence`
- **VelocityInheritance**: `float`
- **VelocitySpread**: `float` [NotReplicated] [Deprecated]
- **WindAffectsDrag**: `bool`
- **ZOffset**: `float`

## Methods

- **Clear**() -> `null`
- **Emit**(`particleCount: int = 16`) -> `null`
- **FastForward**(`numFrames: int`) -> `null`

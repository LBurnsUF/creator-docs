---
title: Sparkles
type: class
superclass: Instance
---

# Sparkles

A particle emitter with the visual aesthetic of sparkles.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

Sparkles is one of several particle-emitting classes. Like other particle
emitters of its kind, Sparkles objects emit particles when parented to a
`Class.BasePart` (such as a `Class.Part`) or an `Class.Attachment` within such
a `Class.BasePart`. Compared to the `Class.ParticleEmitter` class, Sparkles
lacks many different customization properties and special methods, such as
`Class.ParticleEmitter.Lifetime` or `Class.ParticleEmitter:Emit()`. It is
useful to create a quick special effect in a pinch; for more detailed work it
is preferable to use a `Class.ParticleEmitter` instead.

When `Class.Sparkles.Enabled` is toggled off, particles emit by this object
will continue to render until their lifetime expires. When a Sparkles object's
`Class.Instance.Parent` is set to `nil` (and/or `Class.Instance:Destroy()`ed),
all particles will instantly disappear. If this effect is not desired, try
hiding the parent object at a far away position, then removing the Sparkles
after a few seconds using `Class.Debris` to give the last particles a chance
to expire. This object does not have a `Class.ParticleEmitter:Clear()` method,
but it is possible to set the `Class.Instance.Parent` to `nil` and back to the
exact same object for the same effect.

Sparkles particles are only emitted from the center of `Class.BasePart` to
which they are parented. Parenting a Sparkles object to an `Class.Attachment`
instead allows customization of the particles' start position.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Sparkles.Color` | `Datatype.Color3` | [Hidden] [NotReplicated] |
| `Class.Sparkles.Enabled` | `bool` |  |
| `Class.Sparkles.LocalTransparencyModifier` | `float` | [Hidden] [NotReplicated] |
| `Class.Sparkles.SparkleColor` | `Datatype.Color3` |  |
| `Class.Sparkles.TimeScale` | `float` |  |

## Methods

### `Class.Sparkles:FastForward`

``FastForward(numFrames: `int`)`` -> `null`
   {security: RobloxScriptSecurity}

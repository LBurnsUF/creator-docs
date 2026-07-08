---
title: Smoke
type: class
superclass: Instance
---

# Smoke

A particle emitter with the visual aesthetic of smoke.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

Smoke is one of several particle-emitting classes. Like other particle
emitters of its kind, Smoke objects emit particles when parented to a
`Class.BasePart` (such as a `Class.Part`) or an `Class.Attachment` within such
a `Class.BasePart`. Compared to the `Class.ParticleEmitter` class, Smoke lacks
many different customization properties and special methods, such as
`Class.ParticleEmitter.Lifetime` or `Class.ParticleEmitter:Emit()`. It is
useful to create a quick special effect in a pinch; for more detailed work it
is preferable to use a `Class.ParticleEmitter` instead.

When `Class.Smoke.Enabled` is toggled off, particles emit by this object will
continue to render until their lifetime expires. When a Smoke object's
`Class.Instance.Parent` is set to `nil` (and/or `Class.Instance:Destroy()`ed),
all particles will instantly disappear. If this effect is not desired, try
hiding the parent object at a far away position, then removing the Smoke after
a few seconds using `Class.Debris` to give the last particles a chance to
expire. This object does not have a `Class.ParticleEmitter:Clear()` method,
but it is possible to set the `Class.Instance.Parent` to `nil` and back to the
exact same object for the same effect.

Smoke particles are only emitted from the center of `Class.BasePart` to which
they are parented. Parenting a Smoke object to an `Class.Attachment` instead
allows customization of the particles' start position.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Smoke.Color` | `Datatype.Color3` |  |
| `Class.Smoke.Enabled` | `bool` |  |
| `Class.Smoke.LocalTransparencyModifier` | `float` | [Hidden] [NotReplicated] |
| `Class.Smoke.Opacity` | `float` | [NotReplicated] |
| `Class.Smoke.RiseVelocity` | `float` | [NotReplicated] |
| `Class.Smoke.Size` | `float` | [NotReplicated] |
| `Class.Smoke.TimeScale` | `float` |  |

## Methods

### `Class.Smoke:FastForward`

``FastForward(numFrames: `int`)`` -> `null`
   {security: RobloxScriptSecurity}

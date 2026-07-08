---
title: Fire
type: class
superclass: Instance
---

# Fire

A preconfigured particle emitter with the visual aesthetic of fire.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.Fire` is one of several preconfigured particle-emitting classes,
alongside `Class.Smoke`, `Class.Sparkles`, and others. Like the others, it
emits particles when parented to a `Class.BasePart` or an `Class.Attachment`
while `Class.Fire.Enabled|Enabled`. This object is useful to create a quick
visual effect for fire, but for more detailed work it's recommended that you
use a `Class.ParticleEmitter` instead.

Particles emit from the center of the parent in an upward (**+Y**) direction,
but a negative `Class.Fire.Heat|Heat` value may be used to emit particles
downward (**-Y**). Using an `Class.Attachment` as the parent instead of a
`Class.BasePart` allows for the emission position/direction to be modified by
changing the `Class.Attachment.CFrame` or related properties.

`Class.Fire` objects consist of two emitters, each affected in various ways by
the `Class.Fire.Size|Size`, `Class.Fire.Heat|Heat`, `Class.Fire.Color|Color`,
and `Class.Fire.SecondaryColor|SecondaryColor` properties. Particles which
emit from the smaller, secondary emitter have a significantly longer lifetime
(and rise farther) than those emitted by the primary emitter.

When `Class.Fire.Enabled|Enabled` is off, existing particles continue to
render until they expire. However, if the `Class.Fire` object's
`Class.Instance.Parent|Parent` is set to `nil`, all existing particles
immediately disappear, similar to the behavior of
`Class.ParticleEmitter:Clear()`.

`Class.Fire` objects emit no light on their own. To help create a cohesive
environment around a burning object, try adding a `Class.PointLight` with an
orange `Class.Light.Color|Color`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Fire.Color` | `Datatype.Color3` |  |
| `Class.Fire.Enabled` | `bool` |  |
| `Class.Fire.Heat` | `float` | [NotReplicated] |
| `Class.Fire.LocalTransparencyModifier` | `float` | [Hidden] [NotReplicated] |
| `Class.Fire.SecondaryColor` | `Datatype.Color3` |  |
| `Class.Fire.Size` | `float` | [NotReplicated] |
| `Class.Fire.TimeScale` | `float` |  |
| `Class.Fire.size` | `float` | [NotReplicated] [Deprecated] |

## Methods

### `Class.Fire:FastForward`

``FastForward(numFrames: `int`)`` -> `null`
   {security: RobloxScriptSecurity}

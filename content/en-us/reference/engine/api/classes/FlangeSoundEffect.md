---
title: FlangeSoundEffect
type: class
superclass: SoundEffect
---

# FlangeSoundEffect

Creates a sweeping or swooshing effect on a sound.

**Inherits from:** `Class.SoundEffect` > `Class.Instance` > `Class.Object`

## Description

The FlangeSoundEffect creates a sweeping or swooshing effect on the Sound or
SoundGroup it is applied to. It does this by copying the original audio signal
and playing on top of the original but slightly offset and modulated.

Like all other `Class.SoundEffect`, a FlangeSoundEffect can be applied either
to a `Class.Sound` or `Class.SoundGroup` by being parented to either.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.FlangeSoundEffect.Depth` | `float` |  |
| `Class.FlangeSoundEffect.Mix` | `float` |  |
| `Class.FlangeSoundEffect.Rate` | `float` |  |

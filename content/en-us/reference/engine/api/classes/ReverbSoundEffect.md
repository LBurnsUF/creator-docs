---
title: ReverbSoundEffect
type: class
superclass: SoundEffect
---

# ReverbSoundEffect

Reverberates audio, simulating the effect of bouncing off walls in a room.

**Inherits from:** `Class.SoundEffect` > `Class.Instance` > `Class.Object`

## Description

The **ReverbSoundEffect** simulates the effect of sounds bouncing off of
several surfaces (such as walls in a room), which causes several overlapping
echoes that arrive at the listener at slightly offset times.

Like all other `Class.SoundEffect|SoundEffects`, a `Class.ReverbSoundEffect`
can be applied either to a `Class.Sound` or `Class.SoundGroup` by being
parented to either.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ReverbSoundEffect.DecayTime` | `float` |  |
| `Class.ReverbSoundEffect.Density` | `float` |  |
| `Class.ReverbSoundEffect.Diffusion` | `float` |  |
| `Class.ReverbSoundEffect.DryLevel` | `float` |  |
| `Class.ReverbSoundEffect.WetLevel` | `float` |  |

---
title: EqualizerSoundEffect
type: class
superclass: SoundEffect
---

# EqualizerSoundEffect

Controls the volume of incoming audio across three frequency ranges.

**Inherits from:** `Class.SoundEffect` > `Class.Instance` > `Class.Object`

## Description

An equalizer allows for control of the volume of various frequency ranges for
the `Class.Sound` or `Class.SoundGroup` the effect is parented to. This can be
used to highlight particular elements of audio or minimize or outright
eliminate others. The `Class.EqualizerSoundEffect` gives control over three
ranges of frequency: Low, Mid, and High. Their specific frequencies are as
follows:

- Low: 0 - 400 Hz
- Mid: 400 - 4000 Hz
- High: 4000+ Hz

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.EqualizerSoundEffect.HighGain` | `float` |  |
| `Class.EqualizerSoundEffect.LowGain` | `float` |  |
| `Class.EqualizerSoundEffect.MidGain` | `float` |  |

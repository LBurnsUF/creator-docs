---
title: ChorusSoundEffect
type: class
superclass: SoundEffect
---

# ChorusSoundEffect

Makes audio more voluminous by simulating multiple voices playing the same
part.

**Inherits from:** `Class.SoundEffect` > `Class.Instance` > `Class.Object`

## Description

A ChorusSoundEffect simulates the effect of multiple vocals or instruments
playing the same part. It does this by taking the original sound and
overlaying copies of that sound. These copies are not exact matches to the
original but instead vary in pitch slightly. This simulates a real chorus, as
different singers or instruments will have slight variations. This effect can
be applied to either an individual sound or to a sound group by parenting it
to the desired instance.

Like all other `Class.SoundEffect`, a ChorusSoundEffect can be applied either
to a `Class.Sound` or `Class.SoundGroup` by being parented to either.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.ChorusSoundEffect.Depth` | `float` |  |
| `Class.ChorusSoundEffect.Mix` | `float` |  |
| `Class.ChorusSoundEffect.Rate` | `float` |  |

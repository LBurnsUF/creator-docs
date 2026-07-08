---
title: SoundGroup
type: class
superclass: Instance
---

# SoundGroup

A `Class.SoundGroup` is used to manage the volume and sound effects on
multiple `Class.Sound|Sounds` at once. `Class.Sound|Sounds` in the SoundGroup
will have their volume and effects adjusted by the SoundGroup.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

A `Class.SoundGroup` is used to manage the volume and effects on multiple
`Class.Sound|Sounds` at once. Every sound in the sound group will have its
volume adjusted by the group's `Class.SoundGroup.Volume|Volume` property which
acts as a multiplier, meaning a `Class.Sound` with volume `0.5` assigned to a
`Class.SoundGroup` with a volume of `0.5` will have an effective volume of
`0.25`.

If the `Class.SoundGroup` has any `Class.SoundEffect|SoundEffects` as
children, those effects will be applied to all of the `Class.Sound|Sounds` in
the group.

Note that a `Class.Sound` must be added to a `Class.SoundGroup` by setting its
`Class.Sound.SoundGroup|SoundGroup` property, not by simply parenting the
`Class.Sound` to the `Class.SoundGroup`. A `Class.Sound` can only belong to
one `Class.SoundGroup` at a time, although you can nest groups as outlined
[here](../../../sound/groups.md#nesting-soundgroups).

See [Sound Groups](../../../sound/groups.md) for further details on working
with the `Class.SoundGroup` class.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.SoundGroup.Volume` | `float` |  |

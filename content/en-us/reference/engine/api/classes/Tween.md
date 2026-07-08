---
title: Tween
type: class
superclass: TweenBase
---

# Tween

The `Class.Tween` object controls the playback of an interpolation.

**Inherits from:** `Class.TweenBase` > `Class.Instance` > `Class.Object`

## Description

The `Class.Tween` object controls the playback of an interpolation. Creating
and configuring a `Class.Tween` is done with the `Class.TweenService:Create()`
function; `Datatype.Instance.new()` cannot be used for this particular object.

Note that while the configuration of a tween can be accessed after a tween has
been created, it can not be modified. If new goals are needed for an
interpolation, a new `Class.Tween` must be created.

Also note that multiple tweens can be played on the same object at the same
time, but they must not be interpolating the same property. If two tweens
attempt to modify the same property, the initial tween will be cancelled and
overwritten by the most recent tween.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Tween.Instance` | `Class.Instance` | [ReadOnly] [NotReplicated] |
| `Class.Tween.TweenInfo` | `Datatype.TweenInfo` | [ReadOnly] [NotReplicated] |

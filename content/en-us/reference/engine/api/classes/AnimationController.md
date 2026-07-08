---
title: AnimationController
type: class
superclass: Instance
---

# AnimationController

Allows animations to be loaded and applied to a character or model in place of
a `Class.Humanoid`.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

An object which allows animations to be loaded and applied to a character or
model in place of a `Class.Humanoid`. Creates an `Class.Animator` and loads
animations to update `Class.Motor6D|Motor6Ds` of said character to react in
the way that is described within the animation asset referenced by an
`Class.Animation` object.

Note that the `Class.AnimationController:LoadAnimation()|LoadAnimation()`
method of this class has been deprecated. Instead, you should call
`Class.Animator:LoadAnimation()` directly from an `Class.Animator` which can
be created manually in Studio and directly referenced in scripts. When the
deprecated method is called from an `Class.AnimationController`, the
controller itself does nothing regarding the animation intended to be loaded,
except to automatically generate an `Class.Animator`, onto which the loading
call and animation ID are transferred. In this way, the
`Class.AnimationController` can be thought of as nothing more than an empty
shell for a child `Class.Animator` object which handles any actual
functionality regarding animations.

## Methods

### `Class.AnimationController:GetPlayingAnimationTracks`

``GetPlayingAnimationTracks()`` -> `Array`
  [Deprecated]

### `Class.AnimationController:LoadAnimation`

``LoadAnimation(animation: `Class.Animation`)`` -> `Class.AnimationTrack`
  [Deprecated]

## Events

### `Class.AnimationController.AnimationPlayed`

Fires with: (animationTrack: `Class.AnimationTrack`)
  [Deprecated]

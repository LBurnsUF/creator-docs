---
title: Animator
type: class
superclass: Instance
---

# Animator

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.Animator.EvaluationThrottled` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.Animator.PreferLodEnabled` | `bool` |  |
| `Class.Animator.RootMotion` | `Datatype.CFrame` | [ReadOnly] [NotReplicated] [NotBrowsable] |
| `Class.Animator.RootMotionWeight` | `float` | [ReadOnly] [NotReplicated] [NotBrowsable] |

## Methods

### `Class.Animator:ApplyJointVelocities`

``ApplyJointVelocities(motors: `Variant`)`` → `null`

### `Class.Animator:GetPlayingAnimationTracks`

``GetPlayingAnimationTracks()`` → `Array`

### `Class.Animator:GetPlayingAnimationTracksCoreScript`

``GetPlayingAnimationTracksCoreScript()`` → `Array`
   {security: RobloxScriptSecurity}

### `Class.Animator:GetTrackByAnimationId`

``GetTrackByAnimationId(animationId: `Datatype.ContentId`)`` → `Class.AnimationTrack`

### `Class.Animator:LoadAnimation`

``LoadAnimation(animation: `Class.Animation`)`` → `Class.AnimationTrack`

### `Class.Animator:LoadAnimationCoreScript`

``LoadAnimationCoreScript(animation: `Class.Animation`)`` → `Class.AnimationTrack`
   {security: RobloxScriptSecurity}

### `Class.Animator:LoadStreamAnimation`

``LoadStreamAnimation(animation: `Class.TrackerStreamAnimation`)`` → `Class.AnimationStreamTrack`
   {security: RobloxScriptSecurity}

### `Class.Animator:LoadStreamAnimationForSelfieView_deprecated`

``LoadStreamAnimationForSelfieView_deprecated(animation: `Class.TrackerStreamAnimation`, player: `Class.Player`)`` → `Class.AnimationStreamTrack`
   {security: RobloxScriptSecurity}

### `Class.Animator:LoadStreamAnimationV2`

``LoadStreamAnimationV2(animation: `Class.TrackerStreamAnimation`, player: `Class.Player`, shouldLookupPlayer: `bool`, shouldReplicate: `bool`)`` → `Class.AnimationStreamTrack`
   {security: RobloxScriptSecurity}

### `Class.Animator:RegisterEvaluationParallelCallback`

``RegisterEvaluationParallelCallback(callback: `Datatype.Function`)`` → `null`

### `Class.Animator:StepAnimations`

``StepAnimations(deltaTime: `float`)`` → `null`
   {security: PluginSecurity}

### `Class.Animator:StepAnimationsInternal`

``StepAnimationsInternal(deltaTime: `float`, options: `Dictionary`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.Animator:SynchronizeWith`

``SynchronizeWith(otherAnimator: `Class.Animator`)`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.Animator.AnimationPlayed`

Fires with: (animationTrack: `Class.AnimationTrack`)

### `Class.Animator.AnimationPlayedCoreScript`

Fires with: (animationTrack: `Class.AnimationTrack`)

### `Class.Animator.AnimationStreamTrackPlayed`

Fires with: (animationTrack: `Class.AnimationStreamTrack`)

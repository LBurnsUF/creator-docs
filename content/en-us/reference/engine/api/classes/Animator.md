---
title: Animator
type: class
superclass: Instance
---

# Animator

**Inherits**: Instance > Object

## Properties

- **EvaluationThrottled**: `bool` [ReadOnly] [NotReplicated]
- **PreferLodEnabled**: `bool`
- **RootMotion**: `CFrame` [ReadOnly] [NotReplicated] [NotBrowsable]
- **RootMotionWeight**: `float` [ReadOnly] [NotReplicated] [NotBrowsable]

## Methods

- **ApplyJointVelocities**(`motors: Variant`) -> `null`
- **GetPlayingAnimationTracks**() -> `Array`
- **GetPlayingAnimationTracksCoreScript**() -> `Array`
- **GetTrackByAnimationId**(`animationId: ContentId`) -> `AnimationTrack`
- **LoadAnimation**(`animation: Animation`) -> `AnimationTrack`
- **LoadAnimationCoreScript**(`animation: Animation`) -> `AnimationTrack`
- **LoadStreamAnimation**(`animation: TrackerStreamAnimation`) -> `AnimationStreamTrack`
- **LoadStreamAnimationForSelfieView_deprecated**(`animation: TrackerStreamAnimation`, `player: Player`) -> `AnimationStreamTrack`
- **LoadStreamAnimationV2**(`animation: TrackerStreamAnimation`, `player: Player = nil`, `shouldLookupPlayer: bool = true`, `shouldReplicate: bool = true`) -> `AnimationStreamTrack`
- **RegisterEvaluationParallelCallback**(`callback: Function`) -> `null`
- **StepAnimations**(`deltaTime: float`) -> `null`
- **StepAnimationsInternal**(`deltaTime: float`, `options: Dictionary`) -> `null`
- **SynchronizeWith**(`otherAnimator: Animator`) -> `null`

## Events

- **AnimationPlayed**(`animationTrack: AnimationTrack`)
- **AnimationPlayedCoreScript**(`animationTrack: AnimationTrack`)
- **AnimationStreamTrackPlayed**(`animationTrack: AnimationStreamTrack`)

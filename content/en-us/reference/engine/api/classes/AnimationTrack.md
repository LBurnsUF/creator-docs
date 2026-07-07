---
title: AnimationTrack
type: class
superclass: Instance
tags: [NotCreatable]
---

# AnimationTrack

**Inherits**: Instance > Object

**Tags**: NotCreatable

## Properties

- **Animation**: `Animation` [ReadOnly] [NotReplicated]
- **IsPlaying**: `bool` [ReadOnly] [NotReplicated]
- **Length**: `float` [ReadOnly] [NotReplicated]
- **Looped**: `bool`
- **Priority**: `AnimationPriority`
- **Speed**: `float` [ReadOnly] [NotReplicated]
- **TimePosition**: `float` [NotReplicated]
- **WeightCurrent**: `float` [ReadOnly] [NotReplicated]
- **WeightTarget**: `float` [ReadOnly] [NotReplicated]

## Methods

- **AdjustSpeed**(`speed: float = 1`) -> `null` [CustomLuaState]
- **AdjustWeight**(`weight: float = 1`, `fadeTime: float = 0.100000001`) -> `null` [CustomLuaState]
- **GetDebugData**() -> `Dictionary`
- **GetMarkerReachedSignal**(`name: string`) -> `RBXScriptSignal`
- **GetParameter**(`key: string`) -> `Variant`
- **GetParameterDefaults**() -> `Dictionary`
- **GetTargetInstance**(`name: string`) -> `Instance`
- **GetTargetNames**() -> `Array`
- **GetTimeOfKeyframe**(`keyframeName: string`) -> `double`
- **Play**(`fadeTime: float = 0.100000001`, `weight: float = 1`, `speed: float = 1`) -> `null` [CustomLuaState]
- **ResetGraph**() -> `null`
- **SetParameter**(`key: string`, `value: Variant`) -> `null`
- **SetTargetInstance**(`name: string`, `target: Instance`) -> `null`
- **Stop**(`fadeTime: float = 0.100000001`) -> `null` [CustomLuaState]
- **UpdateGraphNodeProperty**(`nodeId: string`, `propertyName: string`, `value: Variant`, `inputPinName: string = `) -> `bool`

## Events

- **DidLoop**()
- **Ended**()
- **KeyframeReached**(`keyframeName: string`)
- **Stopped**()

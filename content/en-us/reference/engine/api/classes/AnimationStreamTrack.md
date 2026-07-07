---
title: AnimationStreamTrack
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# AnimationStreamTrack

**Inherits**: Instance > Object

**Tags**: NotCreatable, NotReplicated

## Properties

- **Animation**: `TrackerStreamAnimation` [Hidden] [ReadOnly] [NotReplicated]
- **FACSDataLod**: `FACSDataLod` [Hidden] [ReadOnly] [NotReplicated]
- **IsPlaying**: `bool` [Hidden] [ReadOnly] [NotReplicated]
- **Priority**: `AnimationPriority` [Hidden] [NotReplicated]
- **WeightCurrent**: `float` [Hidden] [ReadOnly] [NotReplicated]
- **WeightTarget**: `float` [Hidden] [ReadOnly] [NotReplicated]

## Methods

- **AdjustWeight**(`weight: float = 1`, `fadeTime: float = 0.100000001`) -> `null`
- **GetActive**() -> `bool`
- **GetTrackerData**() -> `Tuple`
- **Play**(`fadeTime: float = 0.100000001`, `weight: float = 1`) -> `null`
- **Stop**(`fadeTime: float = 0.100000001`) -> `null`
- **TogglePause**(`paused: bool`) -> `null`

## Events

- **Stopped**()

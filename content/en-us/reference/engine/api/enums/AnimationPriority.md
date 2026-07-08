---
title: AnimationPriority
type: enum
---

# `Enum.AnimationPriority`

The AnimationPriority Enum determines how concurrently-playing AnimationTracks
contribute to the final animation.

When multiple `Class.AnimationTrack|AnimationTracks` are played concurrently
by the same `Class.Animator` and affect the same animated joints, the tracks
are evaluated in order from high to low priority, per joint, while the total
track weight sum remains less than 1.0. When the track weight sum reaches or
exceeds 1.0 for a joint, evaluation stops and no lower-priority tracks will be
evaluated for that joint. `Class.AnimationTrack|AnimationTracks` with the same
priority that are playing concurrently will blend proportional to their track
weights (normalized if the sum exceeds 1).

Higher priority animation will override lower priority ones per joint. The
priority order is:

1. **Action4**
2. **Action3**
3. **Action2**
4. **Action**
5. **Movement**
6. **Idle**
7. **Core**

Roblox's default character animations, including catalog animation bundles,
play at **Core** priority. **Idle** through **Action4** priority are for
developer use.

The `Enum.AnimationPriority` enum has 7 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.AnimationPriority.Idle` | 0 | (6) - Recommended priority for character idle animations. |
| `Enum.AnimationPriority.Movement` | 1 | (5) - Recommended priority for walk, run, swim, climb, and other locomotion animations. |
| `Enum.AnimationPriority.Action` | 2 | (4) - Recommended priority for character actions that must override idle and locomotion animations. |
| `Enum.AnimationPriority.Action2` | 3 | (3) - Action2 will override Action. |
| `Enum.AnimationPriority.Action3` | 4 | (2) - Action3 will override Action2. |
| `Enum.AnimationPriority.Action4` | 5 | (1) - Action4 is the highest priority available, overriding all other priority values. |
| `Enum.AnimationPriority.Core` | 1000 | (7) - Lowest priority, intended for use by Roblox default animations and catalog animation bundles. |

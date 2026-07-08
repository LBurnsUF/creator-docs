---
title: RollOffMode
type: enum
---

# `Enum.RollOffMode`

How `Class.Sound|Sounds` parented to a `Class.BasePart` or `Class.Attachment`
attenuate (fade out) as the distance between the listener and the parent
increases.

Enum which determines how `Class.Sound|Sounds` parented to a `Class.BasePart`
or `Class.Attachment` attenuate (fade out) as the distance between the
listener and the parent increases.

The `Enum.RollOffMode` enum has 4 item(s).

| Name | Value | Description |
|------|-------|-------------|
| `Enum.RollOffMode.Inverse` | 0 | Volume attenuates from `Class.Sound.RollOffMinDistance` in an inverse manner, mirroring how sounds a |
| `Enum.RollOffMode.Linear` | 1 | Volume attenuates between `Class.Sound.RollOffMinDistance` and `Class.Sound.RollOffMaxDistance` with |
| `Enum.RollOffMode.LinearSquare` | 2 | Volume attenuates between `Class.Sound.RollOffMinDistance` and `Class.Sound.RollOffMaxDistance` with |
| `Enum.RollOffMode.InverseTapered` | 3 | A hybrid model which follows the `Inverse` model when close to `Class.Sound.RollOffMinDistance` and  |

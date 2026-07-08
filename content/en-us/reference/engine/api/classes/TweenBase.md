---
title: TweenBase
type: class
superclass: Instance
tags: [NotCreatable, NotBrowsable]
---

# TweenBase

Abstract base class for in-between interpolation handlers. `Class.Tween`
inherits from `Class.TweenBase`.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotBrowsable]

## Description

Abstract base class for in-between interpolation handlers; parent class of
`Class.Tween`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.TweenBase.PlaybackState` | `Enum.PlaybackState` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.TweenBase:Cancel`

``Cancel()`` -> `null`

### `Class.TweenBase:Pause`

``Pause()`` -> `null`

### `Class.TweenBase:Play`

``Play()`` -> `null`

## Events

### `Class.TweenBase.Completed`

Fires with: (playbackState: `Enum.PlaybackState`)
